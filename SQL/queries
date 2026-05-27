SELECT COUNT(*) AS total_customers
FROM customer_summary;

SELECT * from customer_summary limit 10;



-- What % of customers are leaving?
SELECT churn_flag, COUNT(*) AS customers,
ROUND(COUNT(*) * 100.0 / SUM(COUNT(*)) OVER (), 2) AS percentage
FROM customer_summary
GROUP BY churn_flag;



-- How much on average a customer spends?
SELECT ROUND(AVG(debit_amount), 2) as Avg_spend
from customer_summary;



-- Which customer segement exist ?
SELECT spend_segment, COUNT(*) AS customers,
ROUND(AVG(debit_amount),2) AS avg_spend,
ROUND(AVG(savings_ratio),2) AS avg_savings
FROM customer_summary
GROUP BY spend_segment
ORDER BY avg_spend DESC;



-- Which customers segment are churning more ?
SELECT spend_segment, churn_flag,
COUNT(*) AS customers
FROM customer_summary
GROUP BY spend_segment, churn_flag
ORDER BY spend_segment;



-- DO high income customers behave differently ?
SELECT income_range,
ROUND(AVG(debit_amount),2) AS avg_spend,
ROUND(AVG(savings_ratio),2) AS avg_savings,
ROUND(AVG(transaction_count),2) AS avg_txn
FROM customer_summary
GROUP BY income_range
ORDER BY avg_spend DESC;




-- Which age group is more valuable ?
SELECT age_group,
COUNT(*) AS customers,
ROUND(AVG(debit_amount),2) AS avg_spend
FROM customer_summary
GROUP BY age_group
ORDER BY avg_spend DESC;



-- Which channel is most used ?
SELECT channel,
COUNT(*) AS transactions,
ROUND(SUM(amount),2) AS total_amount
FROM transactions
GROUP BY channel
ORDER BY total_amount DESC;




-- Where do customers spend most ?
SELECT category,
ROUND(SUM(amount),2) AS total_spend
FROM transactions
WHERE transaction_type = 'Debit'
GROUP BY category
ORDER BY total_spend DESC;



-- 

