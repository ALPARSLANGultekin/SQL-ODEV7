# SQL-ODEV7

##film tablosunda bulunan filmleri rating değerlerine göre gruplayınız.
SELECT RATING,COUNT(*) FROM FILM GROUP BY RATING;

##film tablosunda bulunan filmleri replacement_cost sütununa göre grupladığımızda film sayısı 50 den fazla olan replacement_cost değerini ve karşılık gelen film sayısını sıralayınız.
SELECT REPLACEMENT_COST,COUNT(*) FROM FILM GROUP BY REPLACEMENT_COST HAVING COUNT(REPLACEMENT_COST) > 50;

##customer tablosunda bulunan store_id değerlerine karşılık gelen müşteri sayılarını nelerdir?
SELECT STORE_ID,COUNT(CUSTOMER_ID) FROM CUSTOMER GROUP BY STORE_ID;

##city tablosunda bulunan şehir verilerini country_id sütununa göre gruplandırdıktan sonra en fazla şehir sayısı barındıran country_id bilgisini ve şehir sayısını paylaşınız.
SELECT COUNTRY_ID,COUNT(CITY) FROM CITY GROUP BY COUNTRY_ID ;
