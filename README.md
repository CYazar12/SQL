# SQL Ödev 1 | WHERE ve Karşılaştırma &amp; Mantıksal Operatörleri

1-) film tablosunda bulunan title ve description sütunlarındaki verileri sıralayınız.

SELECT description, title FROM film;

![image](https://github.com/CYazar12/SQL/assets/109551508/8f307d7b-37d1-429b-818d-4eca3d212d09)

2-) film tablosunda bulunan tüm sütunlardaki verileri film uzunluğu (length) 60 dan büyük VE 75 ten küçük olma koşullarıyla sıralayınız.

SELECT*FROM film WHERE length >60 AND length <75;

![image](https://github.com/CYazar12/SQL/assets/109551508/5764fcc2-79e9-42bc-9efd-a6a9beedcad1)

3-) film tablosunda bulunan tüm sütunlardaki verileri rental_rate 0.99 VE replacement_cost 12.99 VEYA 28.99 olma koşullarıyla sıralayınız.

SELECT * FROM film
WHERE rental_rate = 0.99 AND replacement_cost = 12.99 
OR replacement_cost = 28.99;

![image](https://github.com/CYazar12/SQL/assets/109551508/ebe65c94-abd0-40c8-904c-97d4a154259a)

4-) customer tablosunda bulunan first_name sütunundaki değeri 'Mary' olan müşterinin last_name sütunundaki değeri nedir?

SELECT last_name FROM customer
WHERE first_name = 'Mary';

![image](https://github.com/CYazar12/SQL/assets/109551508/01f26464-0dda-49e7-a939-044b1b16508c)

5-) film tablosundaki uzunluğu(length) 50 ten büyük OLMAYIP aynı zamanda rental_rate değeri 2.99 veya 4.99 OLMAYAN verileri sıralayınız.

SELECT * FROM film
WHERE length <= 50 
AND NOT (rental_rate = 2.99 OR rental_rate = 4.99);


![image](https://github.com/CYazar12/SQL/assets/109551508/290ea948-b8e9-43d1-83b6-e8702901f4c9)





