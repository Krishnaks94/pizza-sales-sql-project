# Pizza Sales Data Analysis Project
This project is a structured SQL-based analysis of a pizza sales dataset. Below is a detailed breakdown of the steps undertaken:

## Step 1: Understanding the Dataset
The dataset comprises four interconnected tables. Understanding the structure and relationships between these tables is critical:

### orders:
Fields: order_id, order_time, order_date.
Purpose: Tracks when orders were placed.

### order_details:
Fields: order_details_id, order_id, pizza_id, quantity.
Purpose: Links orders to specific pizzas and their quantities.

### pizzas:
Fields: pizza_id, size, price, pizza_type_id.
Purpose: Stores pizza details, including size and pricing.

### pizza_types:
Fields: pizza_type_id, name, category.
Purpose: Provides pizza type names and their categories.

### Key Relationships:
orders and order_details are linked by order_id.
order_details and pizzas are linked by pizza_id.
pizzas and pizza_types are linked by pizza_type_id.

## Step 2: Basic Queries for Initial Insights
The first set of SQL queries focuses on fundamental statistics to understand order volumes and preferences:

### Calculate Total Orders:
Query: Count the total number of orders in the orders table.
Insight: Understand the overall order frequency.

### Calculate Total Revenue:
Query: Sum the product of quantity and price from order_details and pizzas.
Insight: Measure the total sales generated.

### Identify the Highest-Priced Pizza:
Query: Fetch the pizza with the maximum price.
Insight: Highlight premium offerings.

### Determine the Most Popular Pizza Size:
Query: Count orders grouped by pizza size.
Insight: Customer preference for pizza sizes.

### Top 5 Most Ordered Pizza Types:
Query: Aggregate quantity of each pizza type.
Insight: Recognize best-sellers to optimize production.

## Step 3: Intermediate Queries for Deeper Insights
Once basic insights are obtained, intermediate queries explore trends and patterns:

### Total Quantity Ordered by Pizza Category:
Query: Aggregate quantity by pizza category.
Insight: Evaluate demand across categories (e.g., vegetarian vs. meat).

### Order Distribution by Hour:
Query: Group orders by the hour in order_time.
Insight: Pinpoint peak ordering times for staffing and delivery optimization.

### Category-Wise Pizza Count:
Query: Count pizzas grouped by category.
Insight: Assess diversity and balance in product offerings.

### Average Orders per Day:
Query: Calculate the daily average of pizzas sold.
Insight: Measure business activity trends over time.

### Top 3 Pizza Types by Revenue:
Query: Aggregate and rank pizza types based on revenue.
Insight: Understand which items contribute the most to revenue.

## Step 4: Advanced Queries for Strategic Insights
The advanced queries leverage SQL's analytical functions for in-depth evaluations:

### Percentage Revenue Contribution by Pizza Type:
Query: Calculate each pizza type's revenue share of the total sales.
Insight: Identify key drivers of overall revenue.

### Cumulative Revenue Over Time:
Query: Use a window function to compute cumulative sales by order_date.
Insight: Observe revenue growth trends to assess business performance.

### Top 3 Pizzas by Revenue in Each Category:
Query: Rank pizzas within each category by revenue contribution.
Insight: Spotlight high-performing items across different categories.

## Step 5: Drawing Business Insights
Compile insights derived from the queries to inform strategic decisions:

### Customer Preferences:
Popular sizes, categories, and specific pizzas preferred by customers.

### Sales Performance:
Peak sales hours, top revenue contributors, and overall revenue trends.

### Operational Adjustments:
Align staffing and inventory based on ordering patterns and top-performing pizzas.

### Conclusion
The Pizza Sales Data Analysis project demonstrates the power of SQL in analyzing business data to uncover actionable insights. By examining order trends, revenue, and customer preferences, it revealed key patterns, such as popular pizza sizes, top-performing categories, and timing trends, offering valuable input for business optimization. This project underscores the importance of data-driven decisions and provides aspiring analysts with a practical resource to sharpen their SQL skills.
