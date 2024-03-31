MySQL kullandığım için PostgreSQL Sample Database DVD Rental yerine MySQL Sample Database ile yaptım

`Question 1:` customers tablosunda bulunan customerNumber ve customerName sütunlarındaki verileri sıralayınız.
```
    SELECT customerNumber, customerName FROM customers;
```
`Question 2:` customers tablosunda bulunan tüm sütunlardaki verileri customerNumber 160 dan büyük ve 175 ten küçük olma koşullarıyla sıralayınız.
```
    SELECT * FROM customers WHERE customerNumber > 160 AND customerNumber >175;
```
`Question 3:` customers tablosunda bulunan tüm sütunlardaki verileri salesRepEmployeeNumber 1401 ve creditLimit 0 veya 81100 olma koşullarıyla sıralayınız.
```
    SELECT * FROM customers WHERE salesRepEmployeeNumber=1401 AND (creditLimit=0 OR creditLimit=81100);
```
`Question 4:` employees tablosunda bulunan firstName sütunundaki değeri 'Mary' olan müşterinin lastName sütunundaki değeri nedir?
```
    SELECT lastName FROM employees WHERE firstName="Mary";
```
`Question 5:` orderdetails tablosundaki priceEach değeri 50'den büyük olmayıp aynı zamanda orderLineNumber değeri 11 veya 1 olmayan verileri sıralayınız.
```
    SELECT * FROM orderdetails WHERE priceEach <= 50 AND NOT (orderLineNumber = 1 OR orderLineNumber = 11);

```