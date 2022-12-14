## Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.<br />

#### 1- Film tablosunda bulunan filmleri rating değerlerine göre gruplayınız. .<br />

```SQL

SELECT rating, COUNT(title) FROM film 
GROUP BY rating; 
```


#### 2- Film tablosunda bulunan filmleri replacement_cost sütununa göre grupladığımızda film sayısı 50 den fazla olan replacement_cost değerini ve karşılık gelen film sayısını sıralayınız.  <br />

```SQL
SELECT replacement_cost, COUNT(*) FROM film 
GROUP BY replacement_cost 
HAVING COUNT(*)>50; 
```


#### 3- Customer tablosunda bulunan store_id değerlerine karşılık gelen müşteri sayılarını nelerdir?   <br />

```SQL
SELECT store_id , COUNT(*) FROM customer 
GROUP BY store_id;  
```


#### 4-City tablosunda bulunan şehir verilerini country_id sütununa göre gruplandırdıktan sonra en fazla şehir sayısı barındıran country_id bilgisini ve şehir sayısını paylaşınız. <br />

```SQL
SELECT country_id, COUNT(city) FROM city
GROUP BY country_id 
ORDER BY count DESC 
LIMIT 1;  
```
