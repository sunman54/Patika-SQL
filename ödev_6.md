## Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.<br />

#### 1- film tablosunda bulunan rental_rate sütunundaki değerlerin ortalaması nedir ? <br />

```SQL
SELECT AVG(rental_rate) FROM film;
 
```



#### 2- film tablosunda bulunan filmlerden kaç tanesi 'C' karakteri ile başlar ? <br />

```SQL
SELECT COUNT(*) FROM film 
WHERE title LIKE 'C%';
 
```

#### 3- film tablosunda bulunan filmlerden rental_rate değeri 0.99 a eşit olan en uzun (length) film kaç dakikadır ? <br />

```SQL
SELECT MAX(length) FROM film 
WHERE rental_rate IN(0.99);
 
```

#### 4- film tablosunda bulunan filmlerin uzunluğu 150 dakikadan büyük olanlarına ait kaç farklı replacement_cost değeri vardır ? <br />

```SQL
 SELECT COUNT(DISTINCT replacement_cost) FROM film 
 WHERE length>150;
 
```
