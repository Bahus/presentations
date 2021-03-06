# BEGIN;

# Django ORM Best Practices

Сборник советов для web-разработчиков, который поможет избежать некоторых подводных камней при работе с Django-ORM  в связке с PostgreSQL.

> Все используемые в данной презентации фрагменты кода являются выдуманными и используются только в качестве примеров.

Контекст:

* Django == 1.9.*
* PostgreSQL >= 9.4
* Python >= 2.7.*

Обычно процесс взаимодействия разработчика с ORM состоит из двух этапов:

* Разработка и изменение схемы базы данных (описание моделей и миграции)
* Манипуляция данными (QuerySet'ы, SQL)

#### Общие советы

* [Следуйте Django coding style](follow-coding-style.md)
* [Что нужно знать перед началом работы с СУБД](relational-model-basics.md)

#### Разработка и изменение схемы данных

* [Очевидные ограничения и индексы](indexes-and-constraints.md)
* [Избегайте преждевременной денормализации](denormalization.md)
* [Правильно выбирайте типы и параметры полей](field-types.md)
* [Как выполнить миграцию и не тормознуть СУБД?](do-migrations-right.md)

#### Взаимодействие с данными

* [Прочитайте документацию по ORM или как избежать глупых ошибок](common-orm-pitfalls.md)
* [Профилирование запросов](know-your-queries.md)
* [Транзакции и атомарные операции](transaction-and-atomic.md)
* [Правила хорошего тона при работе с моделями и QuerySet'ами](queryset-tips-and-tricks.md)
* [Выбираем TOP-N элементов в каждой группе](top-n-items.md)
* Реализуем паджинацию правильно
* Храним иерархические данные в БД без лишных запросов
* Свежий взгляд на наследование в ORM
* JSONB vs Entity-Attribute-Value
* Полнотекстовый поиск – это просто

### Идентификаторы

`pass`

# COMMIT;
