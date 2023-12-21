# SQL 50
## Crack SQL Interview in 50 Qs

+ Basic to intermediate SQL topics
+ 50 Essential SQL Questions
+ Best for 1 month prep time


## Select

1. `Recylable and Low Fat Products`


+  Table: Products

| Column Name | Type    |
|-------------|---------|
| product_id  | int     |
| low_fats    | enum    |
| recyclable  | enum    |

- product_id is the primary key (column with unique values) for this table.
- low_fats is an ENUM (category) of type ('Y', 'N') where 'Y' means this product is low fat and 'N' means it is not.
- recyclable is an ENUM (category) of types ('Y', 'N') where 'Y' means this product is recyclable and 'N' means it is not.
 

+ Write a solution to find the ids of products that are both low fat and recyclable.

+ Return the result table in any order.

+ The result format is in the following example.

 

	Example 1:

+ Input: 
  Products table:
| product_id  | low_fats | recyclable |
| 0           | Y        | N          |
| 1           | Y        | Y          |
| 2           | N        | Y          |
| 3           | Y        | Y          |
| 4           | N        | N          |

+ Output: 
| product_id  |
| 1           |
| 3           |

+ Explanation: Only products 1 and 3 are both low fat and recyclable.


2. `Find Customer Referee`

+ Table: Customer

| Column Name | Type    |
| id          | int     |
| name        | varchar |
| referee_id  | int     |

- In SQL, id is the primary key column for this table.
- Each row of this table indicates the id of a customer, their name, and the id of the customer who referred them.
 

+ Find the names of the customer that are not referred by the customer with id = 2.

+ Return the result table in any order.

+ The result format is in the following example.

 

	Example 1:

+ Input: 
  Customer table:
| id | name | referee_id |
| 1  | Will | null       |
| 2  | Jane | null       |
| 3  | Alex | 2          |
| 4  | Bill | null       |
| 5  | Zack | 1          |
| 6  | Mark | 2          |

+ Output: 
| name |
| Will |
| Jane |
| Bill |
| Zack |


3. `Big Countries`

	Table: World

| Column Name | Type    |
| name        | varchar |
| continent   | varchar |
| area        | int     |
| population  | int     |
| gdp         | bigint  |

- name is the primary key (column with unique values) for this table.
- Each row of this table gives information about the name of a country, the continent to which it belongs, its area, the population, and its GDP value.
 

A country is big if:

+ it has an area of at least three million (i.e., 3000000 km2), or
+ it has a population of at least twenty-five million (i.e., 25000000).

- Write a solution to find the name, population, and area of the big countries.

- Return the result table in any order.

- The result format is in the following example.

 

	Example 1:

+ Input: 
	World table:
| name        | continent | area    | population | gdp          |
| Afghanistan | Asia      | 652230  | 25500100   | 20343000000  |
| Albania     | Europe    | 28748   | 2831741    | 12960000000  |
| Algeria     | Africa    | 2381741 | 37100000   | 188681000000 |
| Andorra     | Europe    | 468     | 78115      | 3712000000   |
| Angola      | Africa    | 1246700 | 20609294   | 100990000000 |

+ Output: 
| name        | population | area    |
| Afghanistan | 25500100   | 652230  |
| Algeria     | 37100000   | 2381741 |
4. `Article Views I`
	
	Table: Views

| Column Name   | Type    |
| article_id    | int     |
| author_id     | int     |
| viewer_id     | int     |
| view_date     | date    |

+ There is no primary key (column with unique values) for this table, the table may have duplicate rows.
+ Each row of this table indicates that some viewer viewed an article (written by some author) on some date. 
+ Note that equal author_id and viewer_id indicate the same person.
 

- Write a solution to find all the authors that viewed at least one of their own articles.

- Return the result table sorted by id in ascending order.

- The result format is in the following example.

 

	Example 1:

+ Input: 
	Views table:
| article_id | author_id | viewer_id | view_date  |
| 1          | 3         | 5         | 2019-08-01 |
| 1          | 3         | 6         | 2019-08-02 |
| 2          | 7         | 7         | 2019-08-01 |
| 2          | 7         | 6         | 2019-08-02 |
| 4          | 7         | 1         | 2019-07-22 |
| 3          | 4         | 4         | 2019-07-21 |
| 3          | 4         | 4         | 2019-07-21 |

+ Output: 
| id   |
| 4    |
| 7    |


5. `Invalid Tweets`

	Table: Tweets

| Column Name    | Type    |
| tweet_id       | int     |
| content        | varchar |
+ tweet_id is the primary key (column with unique values) for this table.
+ This table contains all the tweets in a social media app.
 

- Write a solution to find the IDs of the invalid tweets. The tweet is invalid if the number of characters used in the content of the tweet is strictly greater than 15.

- Return the result table in any order.

- The result format is in the following example.

 

	Example 1:

+ Input: 
	Tweets table:
| tweet_id | content                          |
| 1        | Vote for Biden                   |
| 2        | Let us make America great again! |

+ Output: 
| tweet_id |
| 2        |

+ Explanation: 
	Tweet 1 has length = 14. It is a valid tweet.
	Tweet 2 has length = 32. It is an invalid tweet.


## Basic Joins

6. `Replace Employee ID with The Unique Identifier`

7. `Product Sales Analysis I`

8. `Customer Who Visited but Dit Not Make Any Transactions`

9. `Rising Temperature`

10. `Average Time of Process per Machine`

11. `Employee Bonus`

12. `Students and Examinations`

13. `Managers with at least 5 Direct Reports`

14. `Confirmation Rate`


## Basic Aggregate Functions

15. `Not Boring Movies`

16. `Average Selling Price`

17. `Project Employees I`

18. `Percentage of Users Attended a Contest`

19. `Queries Quality and Percentage`

20. `Monthly Transactions I`

21. `Immediate Food Delivery II`

22. `Game Play Analysis IV`


## Sorting and Grouping

23. `Number of Unique Subjects Taught by Each Teacher`

24. `User Activity for the Past 30 Days I`

25. `Product Sales Analysis III`

26. `Classes More Than 5 Students`

27. `Find Followers Count`

28. `Biggest Single Number`

29. `Customers Who Bought All Products`

## Advanced Select and Joins

30. `The Number of Employees Which Report to Each Employee`

31. `Primary Department for Each Employee`

32. `Triangle Judgement`

33. `Consecutive Numbers`

34. `Product Price at a Given Date`

35. `Last Person to Fit in the Bus`

36. `Count Salary Categories`

## Subqueries

37. `Employees Whose Manager Left the Company`

38. `Exchange Seats`

39. `Movie Rating`

40. `Restaurant Growth`

41. `Friend Requests II: Who Has the Most Friends`

42. `Investments in 2016`

43. `Department Top Three Salaries`

## Advanced String Functions / Regex / Clause

44. `Fix Names in a Table`

45. `Patients With a Condition`

46. `Delete Duplicate Emails`

47. `Second Highest Salary`

48. `Group Sold Products By The Date`

49. `List the Products Ordered in a Period`

50. `Find Users With Valid E-Mails`
. 
