# kodluyoruz-Sql
1-film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.
**SELECT DISTINCT f.replacement_cost FROM film f**

2-film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?
**SELECT DISTINCT COUNT(f.replacement_cost) FROM film f**

3-film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?
***SELECT count(*) FROM film f WHERE f.title LIKE 'T%' and f.rating='G'**

4-country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?
***SELECT COUNT(*) FROM country c where LENGTH(country)=5** 

5-city tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?
*****SELECT COUNT(*) FROM city c where c.city ~~* '%r'***