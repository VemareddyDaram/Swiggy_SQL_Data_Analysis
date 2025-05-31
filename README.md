# Swiggy_SQL_Data_Analysis

## Motivation

The project is driven by a desire to explore India’s food delivery industry through Swiggy’s dataset, aiming to uncover insights into customer preferences, restaurant performance, and market trends. It seeks to benefit stakeholders like restaurant owners and Swiggy strategists by optimizing pricing and menu strategies while enhancing SQL skills through practical data analysis.

## Project Overview

This project analyzes a dataset from Swiggy, India’s prominent food delivery platform, to gain insights into restaurant characteristics, pricing, ratings, and cuisines across various cities. The data resides in a MySQL database (swiggy_project) and is queried using SQL to address 16 specific business questions. These questions explore restaurant distribution, cuisine popularity, cost trends, and dietary preferences, offering a holistic view of Swiggy’s restaurant ecosystem. The project leverages SQL techniques such as aggregations, joins, window functions, and subqueries to extract meaningful patterns and trends.

## Questions/Topics to Answer

The analysis addresses the following questions to derive insights from the Swiggy dataset: 

1. Count of restaurants with a rating greater than 4.5: Identify top-performing restaurants based on customer ratings.



2. Top city with the highest number of restaurants: Determine the city with the largest restaurant presence on Swiggy.



3. Restaurants with "pizza" in their name: Quantify the prevalence of pizza-focused restaurants.



4. Most common cuisine among restaurants: Identify the dominant cuisine type in the dataset.



5. Average rating of restaurants in each city: Analyze customer satisfaction across different cities.



6. Highest-priced item in the 'Recommended' menu category per restaurant: Explore premium offerings in the recommended section.



7. Top 5 most expensive restaurants offering non-Indian cuisine: Highlight high-cost dining options excluding Indian cuisine.



8. Restaurants with cost per person above the overall average: Identify premium restaurants relative to the average cost.



9. Restaurants with the same name in different cities: Detect chains or franchises operating across multiple cities.



10. Restaurant with the most items in the 'Main Course' category: Find restaurants with extensive main course offerings.



11. 100% vegetarian restaurants: List restaurants exclusively offering vegetarian items, sorted alphabetically.



12. Restaurant with the lowest average item price: Identify the most budget-friendly restaurant.



13. Top 5 restaurants with the highest number of menu categories: Highlight restaurants with diverse menu structures.



14. Restaurant with the highest percentage of non-vegetarian food: Identify restaurants catering predominantly to non-vegetarian customers.



15. Most and least expensive cities for dining: Compare dining costs across cities based on cost per person.



16. Top 2 rated restaurants in each city: Identify the best-performing restaurants in each city by rating.


## Clarifications About Table Attributes

The dataset is stored in a single table named swiggy within the swiggy_project database. Below is a detailed description of the table’s attributes, with clarifications for accurate interpretation:

1. restaurant_no (INTEGER, NOT NULL): Unique identifier for each restaurant. Multiple rows may share the same restaurant_no due to multiple menu items.



2. restaurant_name (VARCHAR(50), NOT NULL): Name of the restaurant. Shared names across cities may indicate chains or franchises.



3. city (VARCHAR(9), NOT NULL): City of the restaurant (e.g., Bangalore, Ahmedabad). The short length suggests abbreviated or specific city names.



4. address (VARCHAR(204)): Restaurant address, including detailed location information. Nullable, so some records may lack addresses.



5. rating (NUMERIC(3,1), NOT NULL): Restaurant rating (e.g., 4.3), with one decimal place for precision.



6. cost_per_person (INTEGER): Average cost per person in Indian Rupees. Nullable, indicating potential missing data.



7. cuisine (VARCHAR(49), NOT NULL): Cuisine type(s) offered (e.g., "Biryani, Chinese"). Multiple cuisines may be listed, separated by commas.



8. restaurant_link (VARCHAR(136), NOT NULL): URL to the restaurant’s Swiggy page, providing a unique reference.



9. menu_category (VARCHAR(66)): Category of the menu item (e.g., Main Course, Beverages). Nullable, as some rows may lack this information.



10. item (VARCHAR(188)): Name of the menu item (e.g., "Butter Naan"). Nullable, allowing rows without specific items.



11. price (VARCHAR(12), NOT NULL): Price of the menu item in Indian Rupees, stored as a string (e.g., "75"). Requires casting to numeric (e.g., CAST(price AS DECIMAL)) for calculations.



12. veg_or_nonveg (VARCHAR(7)): Indicates if the item is "Veg" or "Non-veg". Nullable, suggesting some items may lack classification.

## Conclusion

1. Successfully analyzed Swiggy’s restaurant dataset using SQL, addressing 16 diverse questions to uncover insights into restaurant performance, cuisine trends, and pricing dynamics.

2. Demonstrated proficiency in advanced SQL techniques, enhancing the ability to handle complex datasets and derive meaningful business insights.



3. Identified data quality challenges, such as the VARCHAR price column, emphasizing the importance of preprocessing for accurate analysis.



4. Provided actionable insights that could guide Swiggy or restaurant partners in optimizing menu offerings, pricing strategies, and market positioning.



5. Laid a foundation for future enhancements, such as visualizing results with Python/Tableau or integrating real-time data to explore Swiggy’s operational scale.



6. Strengthened data analysis skills, bridging theoretical SQL knowledge with practical application in the context of India’s food delivery industry.


## Learnings from the Project

This project provided significant technical and analytical growth:

1. Mastery of SQL Techniques: Enhanced proficiency in advanced SQL, including window functions (DENSE_RANK), self-joins, subqueries, and conditional aggregations for complex analyses like vegetarian/non-vegetarian percentages.



2. Data Analysis Competence: Developed skills in translating business questions into SQL queries, uncovering trends in cuisine popularity, pricing, and customer satisfaction.



3. Data Quality Management: Recognized the need for data preprocessing, such as casting VARCHAR price to DECIMAL, to ensure accurate calculations and handle nullable fields.



4. Business Insight Generation: Gained the ability to derive actionable insights, such as identifying high-rated restaurants or cost trends, relevant to Swiggy’s operations and restaurant partners.



5. Query Optimization: Learned to use DISTINCT for accurate counts and select appropriate sorting/grouping criteria to improve query precision and efficiency.
