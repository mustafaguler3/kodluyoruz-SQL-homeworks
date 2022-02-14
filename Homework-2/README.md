# kodluyoruz-Sql
1-film tablosunda bulunan tüm sütunlardaki verileri replacement cost değeri 12.99 dan büyük eşit ve 16.99 küçük olma koşuluyla sıralayınız ( BETWEEN - AND yapısını kullanınız.) 
**SELECT * FROM film f where f.rental_rate between 12.99 and 16.99**

2-.actor tablosunda bulunan first_name ve last_name sütunlardaki verileri first_name 'Penelope' veya 'Nick' veya 'Ed' değerleri olması koşuluyla sıralayınız. ( IN operatörünü kullanınız.) 
**SELECT a.first_name,a.last_name FROM actor a where a.first_name IN('Penelope','Nick','Ed')**

3-film tablosunda bulunan tüm sütunlardaki verileri rental_rate 0.99, 2.99, 4.99 VE replacement_cost 12.99, 15.99, 28.99 olma koşullarıyla sıralayınız. ( IN operatörünü kullanınız.) 
**SELECT * FROM film f where f.rental_rate IN(0.99,2.99,4.99) and f.replacement_cost IN(12.99,15.99,28.99)**