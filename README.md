# Pizza-Runner
Problem Statement: the task is to perform exploratory data analysis on the Pizza House Dataset to help Danny optimize his newly established pizza business. The data provided in the dataset required a thorough cleaning before any analysis could be performed.

To clean the data, I first created a new table, Customer_order_temp, from the customer_orders table and removed any null values from the exclusions, extras, and order_time columns. I then repeated the process for the runner_orders table, by creating temp table  also converting the data types of the distance, duration, and cancellation columns to decimal, int, and datetime, respectively. 

**THE DATA:**
These datasets are as follows:

**customer_orders**: This table contains a row for each individual pizza that is part of a customer's order. The table includes the pizza_id (which corresponds to the type of pizza ordered) and the exclusions and extras (which represent the ingredient_id values that should be removed from or added to the pizza, respectively).
**runners:** This table includes information about each runner, including their registration_date and runner_id.
**runner_orders:** This table contains details about each order that a runner delivers, including the pickup_time (timestamp at which the runner picks up the freshly cooked pizzas), distance, and duration (related to how far and long the runner had to travel to deliver the order to the respective customer).
**pizza_names:** This table lists the two pizza options available: Meat Lovers and Vegetarian.
**pizza_recipes:** This table shows the ingredients used to make each pizza, with a pizza_id and the corresponding toppings.
**pizza_toppings:** This table includes the name of every ingredient used to make pizzas, sorted by topping_id.
These datasets are provided for the purpose of data cleaning and analysis, with the goal of helping Danny to better direct his runners and optimize Pizza Runner's operations.

**DATA CLEANING:**
|In the runner_orders table, I handled null and empty values in the cancellation column.
Similarly, in the customer_orders table, I dealt with null and empty values in both the exclusions and extras columns.
Additionally, I removed unnecessary spaces in the runner_orders.distance column, where the 'km' unit was previously present.
I also took care of unnecessary spaces in the runner_orders.duration column, where both 'mins' and 'minutes' units were previously present.
Furthermore, I removed extra spaces in the pizza_recipes.toppings, customer_orders.exclusions, and customer_orders.extras columns.

**KEY INSIGHTS**
Identified a surge in runner sign-ups during the first week of the month, indicating a concentrated recruitment or engagement strategy during this period.
Observed variations in pickup time among runners, with Runner 2 exhibiting a longer time and Runner 3 having the quickest delivery time from the store, highlighting operational nuances.
Found a positive correlation between the number of pizzas ordered and preparation time, with a decrease in time taken for each pizza as order counts rise, showcasing an efficient preparation process.
Identified a specific customer (ID '103') with the maximum delivery distance, indicating a potential opportunity for route optimization or tailored delivery strategies.
Noted a range in delivery times from 10 to 40 minutes, emphasizing the importance of optimizing delivery processes for consistent and timely service.

