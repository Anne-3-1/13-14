# 13-14
Анна

1-Поле — это отдельный атрибут или колонка в таблице базы данных, содержащий конкретную информацию о сущности. 

Запись — это строка в таблице, представляющая собой полный набор значений для всех полей. Каждая запись соответствует одной сущности

2-Каждое поле получает свой тип данных для определения формата значений, которые оно может хранить. Это обеспечивает целостность данных и оптимизирует использование памяти. Тип поля также помогает предотвратить ошибки ввода

3-Современные СУБД поддерживают различные типы данных, такие как:

- Целые числа (INT)
  
- Числа с плавающей точкой (FLOAT, DOUBLE)
  
- Строки (VARCHAR, CHAR)
  
- Дата и время (DATE, TIME, DATETIME)
  
- Логические значения (BOOLEAN)
  
- Бинарные данные (BLOB)

4-Ключ таблицы — это поле или набор полей, которые уникально идентифицируют каждую запись в таблице

5-Простой ключ состоит из одного поля, в то время как составной ключ включает несколько полей для уникальной идентификации записей в таблице

6-Ключ — это общее понятие для любых полей, используемых для идентификации записей. Первичный ключ — это особый вид ключа, который используется для уникальной идентификации записей в таблице

7-а) Фамилия — не может быть ключом, так как не уникальна для разных записей (несколько людей могут иметь одинаковую фамилию).
  
- б) Имя — не может быть ключом, так как также не уникально (много людей могут иметь одинаковые имена).

- г) Адрес электронной почты — может быть ключом, так как обычно уникален для каждого пользователя.

- д) Адрес веб-сайта — может быть ключом, если каждый адрес уникален в контексте данной базы данных.

8-Одни и те же данные могут быть ключом в одной ситуации, но не в другой. Например, адрес электронной почты может быть уникальным идентификатором для пользователей, но если у нескольких людей одинаковые адреса почты (например, в разных системах), то он не подходит в другой ситуации

9-Номер записи можно использовать как первичный ключ, если он уникален и идентифицирует каждую запись. Если в таблице есть другое уникальное поле, его использование предпочтительнее, так как номер записи может изменяться при вставке и удалении

10-Известные методы поиска данных:

- Линейный поиск;
  
- Двоичный поиск;
  
- Поиск по индексам;
  
- Поиск с помощью хеширования

11-Линейный поиск проходит по каждому элементу. 

Преимущества:
- Простой в реализации;
- Работает на неотсортированных данных.

Недостатки:
- Низкая скорость (O(n)).

Двоичный поиск применяется к отсортированным данным и разделяет массив пополам.

Преимущества:
- Быстрая скорость (O(log n)).

Недостатки:
- Требует предварительной сортировки данных

12-Индекс — это структура данных, которая ускоряет поиск информации в таблице. Он строится на основе значений одного или нескольких полей таблицы, позволяя быстро находить строки

13-Да, для одной и той же таблицы можно построить несколько индексов. Это помогает оптимизировать поиск по разным полям

14-Индекс позволяет СУБД быстро находить нужные записи, избегая полного сканирования таблицы. Индекс указывает на расположение данных, что ускоряет доступ к ним

15-Целостность базы данных — это степень корректности и надежности хранимых данных

16-Физическая целостность обеспечивается через механизмы резервного копирования и восстановления, поддержание структур файлов и управление памятью. Это предотвращает повреждение данных

17-Логическая целостность достигается через ограничения целостности (например, уникальность, ненулевые значения) и триггеры, которые обеспечивают аккуратность и согласованность данных на уровне логики приложения
