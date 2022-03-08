# Unique-Users-Per-Client-Per-Month
StrataScratch
select client_id,DATE_PART('month',time_id),COUNT(DISTINCT user_id) from fact_events
group by 1,2;
