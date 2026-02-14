-- Convert VARCHAR timestamps to DATETIME
ALTER TABLE olist_orders
ADD purchase_date DATETIME;

UPDATE olist_orders
SET purchase_date = STR_TO_DATE(order_purchase_timestamp, '%Y-%m-%d %H:%i:%s');

-- Handle missing categories
UPDATE olist_products
SET product_category_name = 'Unknown'
WHERE product_category_name IS NULL 
   OR product_category_name = '';
