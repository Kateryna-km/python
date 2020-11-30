# Лабораторна робота №3

**_Варіант 10._** Створити сервіс для календаря подій. 
Користувач має можливість створювати подію, редагувати її, 
видаляти, долучати інших користувачів до події, переглядати 
перелік всіх створених події, та подій до яких він долучений.


**Хід роботи**

1.	Описати структуру бази даних, зробити діаграму з таблицями та зв'язками між ними
2.	Встановити одну з реляційних СУБД, які SQLAlchemy підтримує  (PostgreSQL, MySQL чи іншу)
3.	Створити у базі даних необхідні таблиці за допомогою SQL запитів чи графічного інтерфейсу до обраної СУБД
4.	Створити SQLAlchemy ORM моделі для таблиць та спробувати використати їх для операцій над базою даних
5.	Видалити попередньо створені вручну таблиці та створити автоматично-згенерований скрипт міграції за допомогою Alembic, застосувати створений скрипт міграції


**Створення міграцій за допомогою SQLAlchemy**
Міграції були створені за допомогою наступних команд:
- python app.py db init
- python app.py db migrate
- python app.py db upgrade


**Таблиці:** 

*Подія* </br>
- id </br>
- назва </br>
- дата </br>
- автор події </br>

*Користувач*</br>
- id </br>
- нікнейм </br>
- ім'я </br>
- прізвище </br>
- e-mail </br>
- пароль </br>
- номер телефону </br>

*Календар*</br>
- id </br>
- доданий користувач </br>
- подія </br>

