1-city tablosu ile country tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz LEFT JOIN sorgusunu yazınız.


**SELECT c.country,cty.city FROM country c
Left Join city cty on cty.country_id = c.country_id**

2-customer tablosu ile payment tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz RIGHT JOIN sorgusunu yazınız.


**SELECT p.payment_id,c.first_name,c.last_name FROM customer c
Right Join payment p on p.customer_id = c.customer_id**

3-customer tablosu ile rental tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name 
isimlerini birlikte görebileceğimiz FULL JOIN sorgusunu yazınız.


**SELECT r.rental_id,c.first_name,c.last_name FROM customer c
Full Join rental r on r.customer_id = c.customer_id**