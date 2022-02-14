1-film tablosunda film uzunluğu length sütununda gösterilmektedir. Uzunluğu ortalama film uzunluğundan fazla kaç tane film vardır?

***SELECT COUNT(*) FROM film f
where f.length > ANY (select AVG(f.length) from film f)**


2-film tablosunda en yüksek rental_rate değerine sahip kaç tane film vardır?


***SELECT COUNT(*) FROM film f
where f.rental_rate = ANY (select MAX(f.rental_rate) from film f)**


3-film tablosunda en düşük rental_rate ve en düşün replacement_cost değerlerine sahip filmleri sıralayınız.


***SELECT COUNT(*) FROM film f
where f.rental_rate = ANY (select MIN(f.rental_rate) from film f) AND f.replacement_cost = ANY (select MIN(f.replacement_cost) from film f)**



4-payment tablosunda en fazla sayıda alışveriş yapan müşterileri(customer) sıralayınız.


**SELECT c.first_name,c.last_name FROM customer c
Inner Join payment p on p.customer_id= c.customer_id
where p.amount = any (select MAX(p.amount) from payment p)**