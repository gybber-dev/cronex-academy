---
title: "Введение в конфиденциальные транзакции"
description: "Конфиденциальные транзакции - инновационный механизм в криптовалютах, обеспечивающий скрытность передаваемых данных и адресов участников сети. Этот метод способствует повышению уровня конфиденциальности и анонимности транзакций."
level: "advanced"
coverImage: "/assets/blog/introduction-to-confidential-transactions/cover.png"
date: "2023-12-04T05:35:07.322Z"
time: 4
ogImage:
  url: "/assets/blog/introduction-to-confidential-transactions/cover.png"
tags:
  - cryptocurrency
  - security
  - technology
---


## Введение
Эффективная работа блокчейна во многом зависит от прозрачности системы. Каждая узел в сети имеет возможность хранить копию блокчейна и проверять его соответствие правилам. В различных децентрализованных реестрах пользователи имеют возможность загружать онлайн-обозреватели блоков для поиска информации о блоках, транзакциях и адресах.

Однако конфиденциальность этой структуры далека от совершенства. В системах, таких как биткоин, каждая транзакция связана с предыдущей. Важно отметить, что монеты технически не являются взаимозаменяемыми, поскольку каждая из них может быть прослежена до конкретных транзакций. Хотя невозможно запретить отправку биткоинов, сеть может отказаться от проведения транзакции, если обнаружит, что ранее использованный адрес находится в черном списке.

В худшем случае отсутствие взаимозаменяемости может существенно повлиять на основы всей системы. Новые монеты могут иметь большую ценность, в то время как старые, учитывая их историю, могут оказаться менее привлекательными для использования.

Конфиденциальность биткоина часто преувеличивают. Отслеживаются не только монеты, но и пользователи. Механизм этой криптовалюты предполагает использование псевдонимов (публичных адресов вместо имен), однако этот подход не лишен недостатков. Сложные методы анализа могут точно связывать адреса, создавая кластеры в попытке деанонимизировать участников сети.

Одним из предлагаемых улучшений было внедрение конфиденциальных транзакций для достижения реальной приватности при проведении операций.

<!-- banner_place -->

## Что такое конфиденциальные транзакции?
Конфиденциальные транзакции (CT) - это концепция, предложенная впервые генеральным директором Blockstream Адамом Бэком в 2013 году, а затем дополненная идеями биткоин-разработчика Грегори Максвелла. Идея этих транзакций состоит в том, чтобы скрыть информацию о сумме переводов от всех участников сети, кроме двух сторон, участвующих в самой транзакции.

<img src="/assets/blog/introduction-to-confidential-transactions/confidential-transaction.png" alt="Конфиденциальные транзакции" />

В обычных условиях, когда транзакции видны всем, узлы легко могут проверить, что сумма, полученная стороной, не превышает отправленную сумму. Например, если Луиза хочет отправить Джону 0,3 BTC, она берет неизрасходованный вывод (например, 1 BTC), отправляет 0,3 BTC Джону, а оставшиеся 0,69 BTC возвращает себе (с учетом комиссии за майнинг).

Однако в случае конфиденциальных транзакций, когда сумма не доступна для просмотра другими участниками сети, проверка становится сложнее. Как можно убедиться, что неизвестное число равно или превышает сумму других неизвестных чисел? Это задача, которая остается вызывающей сложности в контексте конфиденциальных транзакций, и ее решение требует специальных методов шифрования и математических приемов для обеспечения верификации без раскрытия конкретных сумм.

## Обзор используемой криптографии

Для обеспечения конфиденциальности данных важно применять шифрование. Однако традиционные методы подобны помещению информации в сейф: данные становятся недоступными для использования, пока не будут извлечены из сейфа. Для реализации конфиденциальных транзакций необходимо иметь цифровой сейф, в котором содержимое остается скрытым, но его свойства могут быть проверены посторонними лицами.

Гомоморфное шифрование, также известное как обязательство Педерсена, играет ключевую роль в этой концепции. Этот тип шифрования позволяет сторонним лицам проводить операции с зашифрованными данными, не раскрывая их содержание, что имеет множество практических применений.

Традиционный хеш может быть использован для зафиксирования данных, которые вы хотите раскрыть позднее. Допустим, вы проводите конкурс в социальных сетях, где участники должны угадать ваше предпочтение в бирже, чтобы выиграть приз в 0,01 BTC. Для подтверждения честности вы можете предоставить хеш строку, которая указывает на определенный вход данных, скрывая само значение. Это помогает участникам проверить подлинность ответа после объявления результатов.

Однако такой подход не гарантирует абсолютную надежность. Участники могут перебирать возможные варианты, хешируя различные входы и ища соответствия. Для снижения вероятности подобных атак используется ослепляющий фактор - случайные данные, добавляемые к информации для хеширования.

Обязательство Педерсена позволяет объединять данные, сохраняя их конфиденциальность. Этот метод используется в процессе транзакций, где перед отправкой средств создаются обязательства, проверяемые для подтверждения корректности данных при получении.

<img src="/assets/blog/introduction-to-confidential-transactions/formula.png" alt="C(BF1 + D1) + C(BF2 + D2) = C(BF1 + BF2, D1 + D2) Где BF — ослепляющий фактор, а D — данные" />

Хотя этот метод имеет несколько шагов и использует криптографию на эллиптических кривых, основная идея заключается в том, что при проведении транзакции обязательства складываются и проверяются для подтверждения совпадения входных и выходных данных, обеспечивая верификацию транзакции без раскрытия конкретных сумм.

## На что способны конфиденциальные транзакции?
Конфиденциальные транзакции представляют собой механизм, который позволяет скрывать данные о входах и выходах транзакции, обеспечивая более высокий уровень конфиденциальности в системе блокчейн. Если бы такая функциональность была внедрена в протокол биткоина, это значительно повысило бы уровень приватности. Входные и выходные данные стали бы недоступны для общего обозрения, а записи в блокчейне были бы запутаны, однако узлы всё же могли бы проверять подлинность транзакций. Это повышение уровня конфиденциальности позволило бы биткоинам стать взаимозаменяемыми, так как история каждой единицы монеты не раскрывалась бы через анализ цепочки блоков.

Однако интеграция конфиденциальных транзакций в протокол биткоина на данный момент маловероятна. Дополнительная функциональность увеличила бы размер транзакций, что привело бы к большей нагрузке на сеть, учитывая ограниченное пространство блоков. Кроме того, это требовало бы согласия большинства участников на внесение изменений в код протокола, что является сложной и трудоемкой задачей.

Такие изменения могут стать объектом обсуждения и рассмотрения в будущем, но в настоящее время реализация конфиденциальных транзакций в биткоине представляется маловероятной из-за технических и структурных ограничений, а также необходимости широкой поддержки со стороны сообщества и участников сети.

## Резюме
Конфиденциальные транзакции представляют собой интегрированный в другие криптовалюты и сайдчейны биткоина механизм, используемый для обеспечения высокого уровня приватности и конфиденциальности. Например, Monero применяет конфиденциальные транзакции в сочетании с кольцевыми подписями для достижения анонимности и взаимозаменяемости монет. Технология конфиденциальных транзакций также используется в сайдчейне Liquid и MimbleWimble для улучшения уровня конфиденциальности.

Хотя конфиденциальные транзакции обладают множеством преимуществ, включая повышенный уровень конфиденциальности, их применение сопряжено с рядом технических сложностей. В мире криптовалют проблемы масштабируемости и пропускной способности базовых систем являются серьезными ограничениями. Большие объемы транзакций, связанные с конфиденциальными механизмами, могут увеличить нагрузку на сеть и создать проблемы масштабирования.

Однако сторонники конфиденциальности в криптовалютах утверждают, что скрытие сумм транзакций и адресов участников является важным аспектом для обеспечения взаимозаменяемости монет. Они считают, что это необходимо для того, чтобы криптовалюта могла функционировать как деньги, обладающие свойством взаимозаменяемости и обеспечивающие высокий уровень приватности для пользователей.







