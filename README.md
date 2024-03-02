# Стуруктура базы данных для приложения Filmorate.
## Содержание:
1. [Схема базы данных.](https://github.com/Cra5h23/Sprint11DataBase/edit/main/README.md#%D1%81%D1%85%D0%B5%D0%BC%D0%B0-%D0%B1%D0%B0%D0%B7%D1%8B-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85)
2. [Краткое описание всех таблиц.](https://github.com/Cra5h23/Sprint11DataBase/edit/main/README.md#%D0%BA%D1%80%D0%B0%D1%82%D0%BA%D0%BE%D0%B5-%D0%BE%D0%BF%D0%B8%D1%81%D0%B0%D0%BD%D0%B8%D0%B5-%D0%B2%D1%81%D0%B5%D1%85-%D1%82%D0%B0%D0%B1%D0%BB%D0%B8%D1%86)

### Схема базы данных.
![Sprint11DataBAse drawio](https://github.com/Cra5h23/Sprint11DataBase/assets/145023705/e0a3972d-c9da-4ad6-9bd5-4e1d858aa016)

### Краткое описание всех таблиц.
- Таблица films используется для хранения всех фильмов.
  * Поле film_id первичный ключ таблицы, содержит идентификационный номер фильма.
  * Поле rating_id внешний ключ используется для связи с таблицей rating, содержит идентификационный номер рейтинга.
  * Поле name содержит название фильма.
  * Поле description содержит описание фильма.
  * Поле release_date содержит дату релиза фильма.
  * Поле duration содержит продолжительность фильма.
  
- Таблица users используется для хранения всех пользователей.
  * Поле user_id первичный ключ таблицы, содержит идентификационный номер пользователя.
  * Поле email содержит email пользователя.
  * login содержит логин пользователя.
  * name содержит имя пользователя.
  * birthday содержит день рождения пользователя.

- Таблица likes
  * film_id
  * user_id

- Таблицаfilm_ganre

film_id

genre_id
- Таблица rating
PK	rating_id

name
- Таблица friends

user_id
friend_id
- Таблицаgenre
PK	genre_id

name
- Таблицаstatus
PK	status_id
name
- Таблица friend
PK	friend_id
FK	user_id
FK	status_id
