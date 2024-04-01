Bu repo içierisindeki mysqlsampledatabase.sql yani MySQL Sample Database kullanılmıştır.

`Question 1:` customers tablosunda bulunan salesRepEmployeeNumber sütununda bulunan birbirinden farklı değerleri sıralayınız.
```
    SELECT DISTINCT salesRepEmployeeNumber FROM classicmodels.customers;
```
`Question 2:` customers tablosunda bulunan salesRepEmployeeNumber sütununda birbirinden farklı kaç tane veri vardır?
```
    SELECT COUNT(DISTINCT salesRepEmployeeNumber) FROM classicmodels.customers;
```
`Question 3:` customers tablosunda bulunan contactLastName isimlerinden kaç tanesi 'F' karakteri ile başlar ve aynı zamanda country değeri 'USA'e eşittir?
```
    SELECT COUNT(contactLastName) FROM classicmodels.customers WHERE country LIKE "USA" AND contactLastName LIKE "F%";
```
`Question 4:` country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?
```
    SELECT COUNT(DISTINCT country) FROM classicmodels.customers WHERE country LIKE "_____";
```
ya da 
```
    SELECT COUNT(country) FROM classicmodels.customers WHERE LENGTH(country) = 5;
```
`Question 5:` city tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?
```
    SELECT COUNT(DISTINCT city) FROM classicmodels.customers WHERE city LIKE "%D";
```
