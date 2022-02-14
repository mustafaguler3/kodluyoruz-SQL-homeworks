1-Film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir?
**SELECT AVG(rental_rate) FROM film**


2-Film tablosunda bulunan filmlerden kaçtanesi 'C' karekteri ile başlar?
***SELECT COUNT(*) FROM film WHERE title ~~'C%'**


3-Film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır?
**SELECT MAX(length) FROM film WHERE rental_rate = '0.99'**