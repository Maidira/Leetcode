# Leetcode

# Leetcode-SQL 50


Q1. Recyclable and Low Fat Products
 
SELECT product_id
FROM products
WHERE low_fats = 'Y' AND recyclable = 'Y';

-----
Q2. Find Customer Referee

SELECT name
FROM Customer 
WHERE referee_id != 2 OR referee_id IS NULL;

-----
Q3. Big Countries

SELECT 
    name, 
    population, 
    area
FROM World
WHERE 
    population >= 25000000 
    OR area >= 3000000;

-----
Q4. Article Views I

SELECT DISTINCT author_id as id
FROM views
WHERE 
    author_id = viewer_id
ORDER BY author_id ASC;

-----
Q5. Invalid Tweets

SELECT tweet_id
FROM tweets
WHERE LENGTH(content) > 15;

-----
