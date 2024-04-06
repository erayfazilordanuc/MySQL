Bu repo içierisindeki mysqlsampledatabase.sql yani MySQL Sample Database kullanılmıştır.

`Question 1:` customers tablosunda bulunan ve contactFirstName değeri 'n' karakteri ile biten creditLimit değer en fazla 59700 olan tüm verileri sıralayınız.
```
    SELECT * FROM classicmodels.customers WHERE contactFirstName LIKE "%n" AND creditLimit < 59700;
```
`Question 2:` customer tablosunda bulunan contactLastName değeri 'n' karakteri ile biten en az salesRepEmployeeNumber değerine sahip son 5 çalışanı(customer) sıralayınız.
```
    SELECT * FROM classicmodels.customers WHERE contactLastName LIKE "%n" ORDER BY salesRepEmployeeNumber DESC LIMIT 5 OFFSET 21;
```
`Question 3:` customer tablosunda bulunan contactLastName sütununa göre azalan ve salesRepEmployeeNumber 1501 olmak koşuluyla ilk 4 veriyi sıralayınız.
```
    SELECT * FROM classicmodels.customers WHERE salesRepEmployeeNumber = 1501 ORDER BY contactLastName LIMIT 4;
```