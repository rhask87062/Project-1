## Project-1-Group 3: E-commerce Exploratory Data Analysis
Welcome to the E-commerce Exploratory Data Analysis project! This project aims to analyze e-commerce data to uncover insights and trends. Our data comes from Vestiaire Collective where people buy and sell designer fashion with a community of millions of fashion enthusiasts worldwide. This README file provides detailed instructions on how to install and use this project.
## Table of Contents
* Installation
* Usage
* Project Structure
* Examples
* Summary of Analysis
* Contributing
* License
## Installation
**Prerequisites**

Before you begin, ensure you have met the following requirements:

Python 3.8 or higher

pip (Python package installer)

**Create and Clone the repository**

* Create a new repository for this project called Project-1. 
* Clone the Repository
  * git clone https://github.com/lucheuer/Project-1.git
  * cd Project-1
* Inside your local Git repository, add the datafile files from your file downloads.
* Push these changes to GitHub or GitLab.

**Install Dependencies**

Install the required packages using pip:
* import numpy as np
* import pandas as pd
* import matplotlib.pyplot as plt
* import plotly.graph_objects as go
* import plotly.express as px
* import seaborn as sns
* import warnings
* warnings.filterwarnings('ignore')
* import plotly.colors as pc

## Usage

**Jupyter Notebook**

The analysis is performed using Jupyter Notebook. To start Jupyter Notebook, run:
* jupyter notebook
  * Open the notebook 'project-1.ipynb

 **Example Analysis**

 Here's a brief overview of how to run the exploratory data analysis:

 1. Load Data: Load the e-commerce dataset into a DataFrame.
 2. Data Cleaning: Handle missing values, data types, and duplicates.
 3. Exploratory Analysis: Perform univariate, bivariate, multivariate analysis, correlation and causation.
 4. Visualization: Use matplotlib and plotly for data visualization.
 5. Insights: Summarize key findings and insights.

**Project Structure**

![image](https://github.com/user-attachments/assets/b9cc2e62-d4cf-4599-a8a1-aaff45a67aa9)

* data/: Contains raw and processed data files.
* notebooks/: Jupyter Notebooks for analysis.
* scripts/: Python scripts for various stages of the analysis.
* examples/: Examples of analysis results and key findings.
* requirements.txt: Lists the Python packages required for the project.
* README.md: Project documentation.

**Examples**
1. Seasonality/Material

Question: If I were to sell a product what season would I want to focus on? How can this help me with inventory of my store?

Finding: The Findings here show that of the items sold almost 84% of these products fall in the All Season Category. You will see in slides later there is a certain material that is widely sold and supports the All season category sales and put All season on top of products sold. Knowing this you could help you better determine what inventory to have on hand as you would expect better product turnover. 

![image](https://github.com/user-attachments/assets/69cd5f61-92f0-4f61-aa38-bcd4fd2da19f)

2. Top Selling Brand
   
Question -Which brand has the highest number of products sold? Identify the brands that have the lowest number of products sold.What trend can you observe in the sales numbers and market of these brands?

Findings -Gucci is the clear leader with the highest number of products sold, significantly outperforming other brands. Gucci's Market Dominance: Gucci is the top-selling brand with the highest number of products sold, indicating its strong market presence and popularity among consumers. Gradual Decline in Sales: There is a clear trend of decreasing sales numbers from the top brand (Gucci) to the bottom brand (Saint Laurent), showing a hierarchical structure in brand performance. Market Division: The sales distribution indicates that while a few brands dominate the market, there is a significant number of brands with comparable sales figures, suggesting a fragmented market with multiple players. Potential for Growth:  Brands with moderate to low sales have the potential for growth by improving their market strategies, product offerings, or expanding their reach to new customer segments.

![image](https://github.com/user-attachments/assets/fcc09802-0b0e-49ae-9e91-9a3f0d411b15)

3. Top Products by Type
   
Question: If I were to sell a product what would be a top product type based on sales? Would someone buy a 2nd hand shirt?

Finding:The bar chart below shows that T-shirts are by far the best selling products which is mostly considered a All season product and majority were made of cotton based on other charts findings. Sellers are able to sell these 2nd hand T-shirts regardless of what one may actually think partly due to brand we believe. 

![image](https://github.com/user-attachments/assets/12648f0e-b43f-4736-a88e-348bec8a39c8)

4. Gender Target

Question: What are the demographics of buyers on the Vestiaire Collective platform. How should you allocate marketing spend?

Findings: About 60% of buyers on the platform are women. This is consistent with the top product categories.

![image](https://github.com/user-attachments/assets/519a4620-a41d-474c-8228-e1a2e40ac2f4)

5. Top 5 Countries

Question: Of the top 5 countries where sellers had the most success what is the top country and by what percent does it see better success?

Finding: The pie graph show the top 5 countries that sold products are Italy at 37.2%, France 27.3%, United Kingdom 15.4%, Germany 10.2% and United States at 9.97%. These top 5 countries make up about 70% of the whole dataset showing that these sellers typically would do better then others outside of these 5. There is other factors that we know can support these such as gender distribution and location such as there is a level of authenticity of the products where they are sold from such as Italy. 

![image](https://github.com/user-attachments/assets/e006a9ce-af94-4931-974a-e94517f31f43)

6. Top 10 Most Expensive Products

Question: What are the top 10 most expensive products by name, and what trends can be observed regarding the types and prices of these high-end items?

Findings: The dominance of luxury watches is evident in the list, with six out of the top ten most expensive products being high-end watches from prestigious brands such as Audemars Piguet, Patek Philippe, Cartier, Rolex, Chopard, and Hublot. These watches, showcasing significant value, dominate the list. The prices of these luxury items range from approximately $3,000 to $12,000, indicating a substantial variation even among the top ten. Besides watches, the list includes other high-value items such as designer trainers (Jordan x Dior), jeans (Chanel), and a jacket (Celine), highlighting that luxury extends beyond timepieces to fashion apparel. The use of precious metals (gold, steel) in watches and high-quality materials (leather, cotton) in apparel underscores the importance of materials and craftsmanship in the pricing of luxury goods. These findings underline the high market value placed on luxury watches and the diversity of high-end products that consumers are willing to invest in.

![image](https://github.com/user-attachments/assets/cebf8607-cba2-4c90-aae0-e2a8fd157e3a)


**Summary of Analysis**

The vestaire dataset, sourced from Kaggle.com/Vestaire, originally comprised a massive file with 36 columns and 900,514 rows. After focusing on the necessary data, the dataset was reduced to 20 columns and 13,736 rows, now called vestaire_smaller. This reduced dataset, representing 1% of the original size, was analyzed to answer several key questions and derive insights.

Key Findings:

1. Seasonal Sales: Nearly 84% of items sold fall into the All Season category, driven by certain widely sold materials, which helps in determining optimal inventory levels for better turnover.
2. Top Brands: Gucci leads in product sales, significantly outperforming other brands. The trend shows a hierarchical structure from Gucci to lower-performing brands like Saint Laurent, indicating a fragmented market with potential growth for lesser-known brands.
3. Material Preferences: Cotton is the most popular material for all seasons, with polyester trailing behind, indicating a strong consumer preference for cotton in clothing and accessories.
4. Product Distribution: Women's Shoes and Women's Clothing are the most distributed categories, while Women's Accessories are the least. Brands can use this data to prioritize high-demand categories and enhance marketing strategies.
5. Product Condition: Gucci also leads in products sold in "Very good condition," which is the highest-selling condition across all brands, emphasizing the importance of quality in inventory management and marketing.
6. Top Products: T-shirts, especially those made of cotton, are the best-selling items, highlighting the viability of selling second-hand T-shirts.
7. Buyer Demographics: Around 60% of buyers are women, aligning with the top product categories and suggesting targeted marketing strategies.
8. Successful Selling Countries: Italy leads in product sales success at 37.2%, followed by France, the United Kingdom, Germany, and the United States. European countries, particularly Italy and France, dominate in total earnings from sold products.
9. Earnings Ratio: The top four products with the highest earnings ratios include luxury items from Louis Vuitton, Gucci, Burberry, and Dita, indicating consistent profitability across different high-end brands.
10. Top Sellers: The top seller earned $20,000, significantly ahead of others, with a noticeable earnings drop among the top ten, indicating a competitive landscape.
11. Expensive Products: Luxury watches dominate the list of the most expensive products, highlighting the high market value placed on these items.
12. Price by Condition: The highest prices are for items in "never worn, with tag" condition, while the lowest prices are for items in "fair condition."
13. Country Price Patterns: Top-selling countries also show higher price concentrations, with significant price variations indicating potential high earnings for specialty products.

These insights can help in strategic planning, inventory management, and targeted marketing, ultimately driving sales growth and profitability.

## Collaborators

Lucas Heuer - https://github.com/lucheuer

Rebecca Storer - https://github.com/ReccaS

Natalie Brewer - https://github.com/nbrew3000

Michael Sheveland - https://github.com/MichaelSheveland

Russell Haskell - https://github.com/rhask87062

## License
Public
