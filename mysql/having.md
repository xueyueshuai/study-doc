#@ 你想要筛选出订单数量大于等于3的客户，可以这样写：

```
SELECT customer_id, COUNT(*) AS order_count
FROM orders
GROUP BY customer_id
HAVING order_count >= 3;
```