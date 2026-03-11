![Dashboard Preview](DashboardPreview.png)
# -TechBridge-Nigeria-Ltd---2024-Sales-Performance-Analysis
**📄Introduction**

This is a data analysis project for TechBridge Nigeria Ltd, a technology distribution company based in Lagos. They sell electronics and accessories across four regions in Nigeria (North, South, East, West) through three ways: Online, In-Store, and Distributors.

I was given their raw, messy sales data for the year 2024. My job was to clean the data, figure out how the business is doing, and build a dashboard to help the managers make better decisions.

**❓ The Problem**

TechBridge had a lot of sales data, but it was full of mistakes and hard to read. Management could not easily answer simple business questions like:

Are we making money or losing money?

Which sales representatives are doing a great job, and who needs help?

Are customers returning too many products?

Which region and store types are bringing in the most cash?

They needed the data cleaned, connected, and turned into a simple dashboard.

**🛠️ The Analysis (Tasks Completed)**

To solve the problem, I acted as a Junior Data Analyst and completed some specific tasks to clean the data and find answers.

1. Splitting Data (Text to Columns)

A column had bunched-up text separated by lines (e.g., Product|Category|Channel). I used the Text to Columns tool to split this into three clean columns: Product, Category, and Channel.

2. Data Cleaning

Fixed spelling mistakes using Find & Replace (e.g., fixing misspelled regions or statuses).

Removed exact duplicate rows using the Remove Duplicates tool.

Filled in empty, blank cells with the word "N/A" so no data was missing.

Highlighted strange prices (like unit prices under ₦1,000 or over ₦600,000) using Conditional Formatting to catch errors and Corredcted them.

3. Connecting Tables with XLOOKUP

I connected the main sales table to a separate lookup table to grab the Product Category and SKU code.

4. Connecting Tables with INDEX & MATCH

I used another method to pull the "Supplier Name" and "Warranty Months" from the lookup table into my main table.

5. Error Handling

I wrapped all search formulas in an =IFERROR() function. This ensures that if a product is missing, the sheet says "Not Found" instead of showing an ugly #N/A error.

6. DAX Measures

I wrote DAX measures to calculate Total Revenue, Average Order Value, Return Rate, Discount, Quantity Sold, where only orders status is Completed.

7. Building the Dashboard
I created an interactive dashboard that updates automatically, showing:

Key Numbers (KPIs): Total Revenue, Total Orders, Average Order Value, and Return Rate, Discount, Quantity Sold.

**🙋‍♂️ Key Questions & Answers**

Here are the main questions the managers needed answered, and how my project answered them:

**Question**: Which region generates the highest revenue?

Answer: The East region is the winner, bringing in ₦153.9 Million.

**Question**: Which sales channels bring in the most money?

Answer: In-Store sales are the highest (₦202.2 Million), followed by Online (₦156.8 Million).

**Question**: Who are our top performing Sales Reps?

Answer: Yemi Osinbajo is the top seller with ₦63.4 Million, closely followed by Emeka Nwosu with ₦60.1 Million.

**Question**: Are we dealing with high product returns?

Answer: Yes. Out of 424 total orders, 49 were returned. This means the return rate is 23.47%, which is very high and costs the company money.

**💡 Key Insights**

From looking at all the numbers and charts, here is what I discovered:

The East is carrying the company: The East region makes the most money, but the West region is far behind (only ₦63.3 Million).

Returns are a huge problem: A return rate of almost 23.5% means that 1 out of every 4 orders is being sent back by the customer.

Electronics rule the sales: Electronics brought in ₦435.1 Million, while Accessories only brought in ₦27.7 Million. Electronics are the main money-makers.

Distributors are falling behind: People are buying In-Store and Online a lot, but the Distributor channel is the lowest performer (₦99.9 Million).

**🚀 Recommendations**

Based on the data, here is what TechBridge Ltd should do next:

Investigate the High Returns: The company must urgently check why customers are returning so many items. Are the electronics damaged? Is the online delivery taking too long? Fixing this will instantly save the company millions of Naira.

Help the West Region: The West region needs help. The company should train the sales reps in that region or run special marketing ads in the West to boost sales.

Push "In-Store" Accessories: Since people buy mostly Electronics In-Store, the store cashiers should be trained to "upsell". For example, if someone buys a Laptop (Electronic), the cashier should offer them a mouse or a keyboard (Accessory) at a small discount.

Reward Top Sellers: Yemi Osinbajo and Emeka Nwosu are doing a fantastic job. They should be rewarded with bonuses, and perhaps asked to train the reps who are struggling to hit their targets.
