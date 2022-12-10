## Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.<br />

#### 1- Film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.<br />

```SQL
SELECT DISTINCT replacement_cost FROM film
 
```


#### 2- Film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır ?<br />

```SQL
21
```


#### 3- Film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir ?<br />

```SQL
9

SELECT COUNT(*) FROM film
WHERE title LIKE 'T%' AND rating = 'G'
```


#### 4- Country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır ? <br />

```SQL
SELECT COUNT(*) FROM country
WHERE country LIKE '_____'

```


#### 5- City tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter ? <br />

```SQL
SELECT COUNT(*) FROM city
WHERE city ~~* '%r'

```

