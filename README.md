Soru 1 Cevap :
select count(*) from film
where length > (select avg(length) from film) ; <br>
Soru 2 Cevap :
select count(*) from film
where rental_rate = (select max(rental_rate) from film) ; <br>
Soru 3 Cevap :
select title, from film
where rental_rate = (select min(rental_rate) from film) and replacement_cost = (select min(replacement_cost) from film)
order by title ; <br>
Soru 4 Cevap :
select customer_id, count(customer_id) as most_purchases from payment
group by customer_id
order by most_purchases desc ; <br>
