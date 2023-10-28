# Домашнее задание к занятию "`12.3. "Домашнее задание к занятию «SQL. Часть 1»"`" - Овчинников Денис

---

### Задание 1

---
```
select distinct district from address
where district like 'K%a' and district not like '% %'
```

![alt text](https://github.com/Ventilyator/ovchinnikov-homework-netology/blob/main/12.3_SQL-1/img/1.png)

---

### Задание 2

---
```
select payment_id, cast(payment_date as date), amount
from payment
where payment_date between '2005-06-15' and '2005-06-19' and amount > 10.00

```
![alt text](https://github.com/Ventilyator/ovchinnikov-homework-netology/blob/main/12.3_SQL-1/img/2.png)

---

### Задание 3

---
```
select distinct district from address
where district like 'K%a' and district not like '% %'
```

![alt text](https://github.com/Ventilyator/ovchinnikov-homework-netology/blob/main/12.3_SQL-1/img/3.png)

---

### Задание 4

---
```
select lower(last_name) last_name , replace ( lower(first_name), 'll', 'pp') first_name , active
from customer
where first_name = 'KELLY' or first_name = 'WILLIE' and active >0
```

![alt text](https://github.com/Ventilyator/ovchinnikov-homework-netology/blob/main/12.3_SQL-1/img/4.png)

---
