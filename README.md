**Amazon Product Price Tracker Using Web Scraping**

This project automates the process of tracking and analyzing price trends for products listed on Amazon. By utilizing web scraping techniques, the project periodically fetches product data, such as price and title, and stores it in a structured format. The collected data is then used for insights or notifications when prices drop, making it ideal for price-sensitive customers or competitive analysis.

**Project Features**

1) Web Scraping:

    - Leveraged BeautifulSoup and requests libraries to extract product data such as titles and prices.

    - Parsed HTML content from Amazon product pages.

2) Data Storage:

    - Stored the extracted data in a CSV file to maintain a record of daily prices.

    - Appended new data to the CSV to ensure continuous tracking without overwriting previous records.

3) Automation:

    - Implemented an automated workflow using Python's time library to scrape data at regular intervals (daily).

    - Ensured scalability for tracking multiple products by extending the scraping function.

4) Email Notifications:

    - Configured an email notification system using the smtplib library to alert users when the product price drops below a specified threshold.

5) Data Analysis:

    - Used pandas to analyze historical pricing data for trends and insights.

**Key Libraries Used**

  - BeautifulSoup: For parsing HTML and extracting product details.

  - Requests: To connect to Amazon web pages and retrieve HTML content.

  - Pandas: For data manipulation and analysis.

  - Smtplib: For sending email notifications.

**Workflow**

1) Connect to Amazon:

    - Define the URL of the target product.

    - Use requests to fetch the webpage content.

2) Extract Data:

    - Parse the fetched HTML using BeautifulSoup.

    - Identify relevant tags for product title and price.

3) Store Data:

    - Save the extracted data (title, price, date) in a CSV file.

    - Append new records without overwriting.

4) Automate the Process:

    - Implement a loop with a timer to scrape data daily.

    - Continuously update the CSV file.

5) Trigger Notifications:

    - Compare the current price with a predefined threshold.

    - If the price drops, send an email notification to the user.

6) Analyze Data:

    - Load the CSV file into a DataFrame for visualizations and trend analysis.

**Use Cases**

- Price tracking for e-commerce shoppers.

- Competitive analysis for retailers.

- Market research on product pricing trends.


