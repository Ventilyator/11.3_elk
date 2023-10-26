# Домашнее задание к занятию "Работа с данными (DDL/DML)" - Овчинников Денис

---

### Задание 1

---
![alt text](https://github.com/Ventilyator/ovchinnikov-homework-netology/blob/main/12.2_hw/img/1.1.png)

![alt text](https://github.com/Ventilyator/ovchinnikov-homework-netology/blob/main/12.2_hw/img/1.2.png)
---

```
CREATE USER 'sys_temp'@'localhost' IDENTIFIED BY 'password';
```
```
SELECT USER FROM mysql.user;
```
```
GRANT ALL PRIVILEGES on *.* TO 'sys_temp'@'localhost';
```
```
show grants for 'sys_temp'@'localhost';
```
```
mysql -u sys_temp -p < /tmp/sakila-db/sakila-schema.sql
```
```
mysql -u sys_temp -p < /tmp/sakila-db/sakila-data.sql
```
---

### Задание 2

---
```
|Название таблицы | Название первичного ключа|
|-----------------|--------------------------|
|actor            | actor_id                 |
|address          | address_id               |
|category         | category_id              |
|city             | city_id                  |
|countru          | country_id               |
|customer         | customer_id              |
|film             | film_id                  |
|film_actor       | actor_id, film_id        |
|film_category    | film_id, category_id     |
|film_text        | film_id                  |
|inventory        | inventory_id             |
|language         | language_id              |
|payment          | payment_id               |
|rental           | rental_id                |
|staff            | staff_id                 |
|store            | store_id                 |
```
---



