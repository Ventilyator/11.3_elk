# Домашнее задание к занятию "`12.4. "Домашнее задание к занятию «SQL. Часть 2»"`" - Овчинников Денис

---

### Задание 1

---
```
select
s2.first_name, s2.last_name, c2.city, count(c.customer_id )
from store s
join customer c on c.store_id = s.store_id
join staff s2 on s2.store_id = s.store_id
join address a on a.address_id =s.address_id
join city c2 on c2.city_id =a.city_id
group by s.store_id, s2.first_name, s2.last_name, c2.city
having count(c.customer_id) > 300
```

![alt text](https://github.com/Ventilyator/ovchinnikov-homework-netology/blob/main/12.4_SQL-2/img/1.png)

---

### Задание 2

---
```
select count(length) film_id 
from film f 
where length > (select AVG(length) from film)

```
![alt text](https://github.com/Ventilyator/ovchinnikov-homework-netology/blob/main/12.4_SQL-2/img/2.png)

---

### Задание 3

---
```
select month (payment_date), count(rental_id), sum(amount) 
from payment p 
group by month (payment_date) 
order by sum(amount) desc
limit 1
```

![alt text](https://github.com/Ventilyator/ovchinnikov-homework-netology/blob/main/12.4_SQL-2/img/3.png)

---
