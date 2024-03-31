Bu repo içierisindeki mysqlsampledatabase.sql yani MySQL Sample Database kullanılmıştır.

`Question 1:` customers tablosunda bulunan tüm sütunlardaki verileri customerNumber değeri 141 dan büyük eşit ve 177 küçük olma koşuluyla sıralayınız.
```
    SELECT * FROM customers WHERE customerNumber BETWEEN 141 AND 177;
```
`Question 2:` employees tablosunda bulunan firstName ve lastName sütunlardaki verileri firstName 'Loui' veya 'Diane' veya 'Jeff' değerleri olması koşuluyla sıralayınız.
```
    SELECT firstName, lastName FROM classicmodels.employees WHERE firstName IN ("Loui", "Diane", "Jeff");
```
`Question 3:` orderdetails tablosunda bulunan tüm sütunlardaki verileri orderNumber 10119, 10120, 10121 ve quantityOrdered 24, 29, 46 olma koşullarıyla sıralayınız.
```
    SELECT * FROM classicmodels.orderdetails WHERE orderNumber IN (10119, 10120, 10121) AND quantityOrdered IN (24, 29, 46);
```
