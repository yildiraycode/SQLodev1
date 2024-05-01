# SQLodev1
## sql sorguları patika odev 1 ##
**Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.**<br/>
1.film  tablosunda bulunan title ve description sütunlarındaki verileri sıralayınız.<br/><br/>
select title,description from film;<br/><br/><br/>
2.film tablosunda bulunan tüm sütunlardaki verileri film uzunluğu (length) 60 dan büyük VE 75 ten küçük olma koşullarıyla sıralayınız.<br/><br/>
select *from film<br/>
where length>60 and length<75;<br/><br/><br/>
3.film tablosunda bulunan tüm sütunlardaki verileri rental_rate 0.99 VE replacement_cost 12.99 VEYA 28.99 olma koşullarıyla sıralayınız.<br/><br/>
select *from film<br/>
where rental_rate=0.99 and replacement_cost=12.99 or replacement_cost=28.99;<br/><br/><br/>
4.customer tablosunda bulunan first_name sütunundaki değeri 'Mary' olan müşterinin last_name sütunundaki değeri nedir?<br/>
cevap:*Smith*<br/><br/>
select first_name,last_name from customer<br/>
where first_name='Mary';<br/><br/><br/>
5.film tablosundaki uzunluğu(length) 50 ten büyük OLMAYIP aynı zamanda rental_rate değeri 2.99 veya 4.99 OLMAYAN verileri sıralayınız.<br/><br/>
select * from film<br/>
where not(length>50) and not(rental_rate=2.99 or rental_rate=4.99);<br/><br/>
