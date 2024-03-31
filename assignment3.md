Bu repo içierisindeki mysqlsampledatabase.sql yani MySQL Sample Database kullanılmıştır

`Question 1:` customers tablosunda bulunan contactFirstName sütunundaki isimlerden 'B' karakteri ile başlayıp 'n' karakteri ile sonlananları sıralayınız.
```
    SELECT * FROM classicmodels.customers WHERE contactFirstName like "B%n";
```
`Question 2:` customers tablosunda bulunan contactLastName sütunundaki isimlerden en az 6 karakterden oluşan ve sonu 'n' karakteri ile sonlananları sıralayınız.
```
    SELECT contactLastName FROM classicmodels.customers WHERE contactLastName LIKE "%_____n";
```
`Question 3:` customers tablosunda bulunan customerName sütunundaki isimlerden en az 4 adet 'T' ya da 't' karakteri içeren isimleri sıralayınız.
```
    SELECT customerName FROM classicmodels.customers WHERE customerName LIKE "%T%T%T%T%";
```
`Question 3:` customer tablosunda bulunan tüm sütunlardaki verilerden city 'C' karakteri ile başlayan ve uzunluğu 9'dan büyük olan ve customerNumber değeri 161'ten uzun olan verileri sıralayınız.
```
    SELECT * FROM classicmodels.customers WHERE city LIKE "C________%" AND customerNumber > 161;
```
