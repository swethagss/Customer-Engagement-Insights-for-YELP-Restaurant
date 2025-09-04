# Yelp Restaurant Business Analysis

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/ff31f909-c3c5-4972-809b-b9f2164ccb5d" />

## Project Background
Yelp is a web and mobile platform where users can discover, review, and share experiences about local businesses through crowd-sourced reviews. It allows users to submit reviews, photos, and tips, while also browsing ratings and insights from others. Yelp covers a wide range of businesses, from restaurants to services, and offers features like search filters, business profiles, and customer feedback.

## Problem Statement
In a competitive market like the restaurant industry, understanding the factors that influence business success is crucial for stakeholders. Utilizing the Yelp dataset, this project aims to investigate the relationship between user engagement (reviews, tips, and check-ins) and business success metrics (review count, ratings) for restaurants.

## Research Objectives
   <img width="741" height="223" alt="Image" src="https://github.com/user-attachments/assets/ac81fffe-4945-4edd-80e0-5461b4204b59" />
  
## Hypothesis
  - Higher levels of user engagement (more reviews, tips, and check-ins) correlate with higher review counts and ratings for restaurants.
  - Positive sentiment expressed in reviews and tips contributes to higher overall ratings and review counts for restaurants
  - Consistent engagement over time is positively associated with sustained business success for restaurants.

## Data Overview
This dataset is a curated subset of Yelp, containing comprehensive information about businesses across eight major metropolitan areas in the USA and Canada.

The original data is provided by Yelp in the form of six JSON files: **business, review, user, tip, checkin, and photos**. For convenience, these JSON files have been stored in a database to facilitate efficient data retrieval and analysis.

## Executive Summary
The analysis for the Yelp Restaurant business was conducted using **SQLite, Python**. SQLite was utilized through Python to perform the data analysis, generating insights from the dataset, which were then visualized.

## SQLite & Python Analysis, Visualization and Findings

### How many restaurant businesses exist, how many are currently open, and what are the descriptive statistics for review count and star rating? Additionally, which restaurants have the highest number of reviews and the highest ratings?
  - Out of 150K businesses, 52K are in the restaurant industry and 35K of those are currently open

      <img width="596" height="281" alt="Image" src="https://github.com/user-attachments/assets/26ca8e03-4f1b-4a95-9b54-5f50e1c87d4f" />

  - There is no direct correlation between ratings and reviews. The highest rating does not necessarily guarantee the highest number of reviews, and vice versa.
  - Review counts reflects user enagament but not necessarily overall customer satisfaction or business performance
  - Success in the restaurant business is not solely determined by ratings or review counts.

### Do restaurants with higher engagement tend to have higher ratings?
  - Data shows a general avg increase in reviews, checkin count and Tip count as ratings imporve from 1 to 4 stars
  - Restaurants rated 4 stars exhibit the highest engagement across reviews, check-ins and tips, suggesting a peak in user interaction
  - Interestingly, engagement metrics (reviews, check-ins, tips) dip for restaurants rated 4.5 and significantly more at 5 stars.
  - The drop in engagement at 5.0 stars might suggest either a saturation point where fewer customers feel compelled to add their reviews, or a selectivity where only a small, satisfied audience frequents these establishments


      <img width="744" height="536" alt="Image" src="https://github.com/user-attachments/assets/8adaadb4-8f03-4c8e-85ac-a741993e73a1" />

      <img width="1116" height="415" alt="Image" src="https://github.com/user-attachments/assets/5619725f-5372-4cb8-a000-98cef62fac7e" />

### Is there a correlation between the number of reviews, tips, and check-ins for a business?
  - These correlations suggest that user engagement across different platforms (reviews, tips, and check-ins) is interlinked; higher activity in one area tends to be associated with higher activity in others.
  - Businesses should focus on strategies that boost all types of user engagement, as increases in one type of engagement are likely to drive increases in others, enhancing overall visibility and interaction with customers.

      <img width="529" height="419" alt="Image" src="https://github.com/user-attachments/assets/0bb7d926-f796-4f7d-b058-383d36327791" />

### Is there a difference in the user engagement between high-rated and low-rated businesses?
  - Data indicates a clear correlation between higher ratings and increased user engagement across reviews, tips, and check-ins.
  - This pattern underscores the importance of maintaining high service and quality standards, as these appear to drive more reviews, check-ins, and tips, which are critical metrics of customer engagement and satisfaction.
  - Businesses should focus on strategies that boost all types of user engagement, as increases in one type of engagement are likely to drive increases in others, enhancing overall visibility and interaction with customers.

      <img width="398" height="123" alt="Image" src="https://github.com/user-attachments/assets/e6c01e71-ab49-47ae-be55-24a5b36f89e1" />

### How do the success metrics of restaurants vary across different states and cities?
  - Philadelphia emerges as the top city with the highest success score, indicating a combination of high ratings and active user engagement.
  - Following Philadelphia, Tampa, Indianapolis, and Tucson rank among the top cities with significant success scores, suggesting thriving restaurant scenes in these areas
  - The success metrics vary significantly across different states and cities, highlighting regional differences in dining preferences, culinary scenes, and customer engagement levels.
  - Identifying cities with high success scores presents opportunities for restaurant chains to expand or invest further, while areas with lower scores may require targeted efforts to improve ratings and increase user engagement.

      <img width="769" height="459" alt="Image" src="https://github.com/user-attachments/assets/26ad88ca-a8ab-4d46-86bb-c34a139c642e" />

### Is there any difference in engagement of Elite users & non-elite users?
  - Elite users are individuala who have been recognized and awarded the "Elite" status by Yelp for their active and high-quality contributions to the platform, such as frequent and detailed reviews, photos, and check-ins, among other criteria.
  - Although elites make up only 4.59% of users, they contribute about 44% of all reviews
  - Elite users often provide detailed and insightful reviews, which can influence other users perceptions and decisions regarding a business.
  - Reviews from elite users may receive more attention and visibility on the Yelp platform due to their status, potentially leading to higher exposure for businesses.
  - Establishing a positive relationship with elite users can lead to repeat visits and loyalty, as they are more likely to continue supporting businesses they have had good experiences with

<img width="316" height="89" alt="Image" src="https://github.com/user-attachments/assets/9ffbd8db-cbd0-4b1f-aafd-e4269878b633" />

<img width="862" height="367" alt="Image" src="https://github.com/user-attachments/assets/16b1fd27-923f-45bf-8763-38061045b9a1" />

### Busiest hours for restaurants
  - Busiest hours for restaurants is between **4PM and 1AM**
  - Knowing the peak hours allows businesses to optimize their staffing levels and resource allocation during these times to ensure efficient operations and quality service delivery
  - The concentration of user engagement during the evening and night hours suggests a higher demand for dining out during these times, potentially driven by factors such as work schedules, social gatherings, and leisure activities

    <img width="1007" height="582" alt="Image" src="https://github.com/user-attachments/assets/abc3a626-abc9-4ecb-b29e-60890bec5381" />

### How many users have left tips to more businesses than reviews, and how does user engagement vary between leaving tips and reviews?
  - Most users are more likely to leave reviews than tips, indicating that reviews are the preferred form of engagement.
  - A smaller but significant group of users engages equally in leaving both tips and reviews, showing a balanced interaction.
  - Few users prioritize leaving tips over reviews, suggesting that tips are less common but may still offer valuable insights for businesses.
  - Businesses should focus more on encouraging reviews while also recognizing the value of tips as a form of user engagement.

<img width="537" height="381" alt="Image" src="https://github.com/user-attachments/assets/76ccfecc-5d55-4561-939b-f7171ef0bc66" />

### Are there any patterns in user engagement over time for successful businesses compared to less successful ones?
  - Successful businesses,particularly those with higher ratings (above 3.5), exhibit consistent and possibly increasing user engagement over time.
  - High-rated restaurants maintain a steady or growing level of user interaction, indicating strong customer interest and satisfaction.

<img width="645" height="386" alt="Image" src="https://github.com/user-attachments/assets/ac736f72-b159-4588-8968-708c227a5085" />

### Are there any seasonal trends in the user engagement for restaurants?
  - Businesses with ratings above 3.5 show consistent and gradually increasing user engagement.
  - High rated restaurants maintain a steady or growing level of user engagement over time, reflecting ongoing customer interest and satisfaction
  - Tip count is trending downward, while review count is trending upward over time.
  - Seasonality reveals lower engagement during Nov–Mar and higher engagement during Apr–Aug.

<img width="1025" height="436" alt="Image" src="https://github.com/user-attachments/assets/f418fb41-d38b-4dd7-aeb4-7111ae30373d" />

### How does the sentiment of reviews and tips (useful, funny, cool) correlate with the success metrics of restaurants?
  - Engagement signals (useful, cool, and review count) are strongly related → they move together.
  - Success score is mostly influenced by review count, useful count and cool count but not by funny count
  - Businesses with lots of reviews also attract more “useful” and “cool” votes.
  - "Funny" is more of a side effect (entertainment value) and doesn’t directly tie to business success.
  - 👉 A restaurant's success score is mainly driven by review volume & perceived usefulness, not by how funny reviews are.

    <img width="523" height="431" alt="Image" src="https://github.com/user-attachments/assets/c836f22b-fbf6-4929-9d6b-8cdb712a9648" />

## Recommendations
  - Utilizing insights from the analysis of various metrics such as user engagement, sentiment of reviews, peak hours, and the impact of elite users, businesses can make informed decisions to drive success.
  - Understanding customer preferences, behavior, and satisfaction levels is paramount. Businesses should focus on delivering exceptional experiences to meet customer expectations.
  - By leveraging data on peak hours and user engagement, businesses can optimize staffing levels, resource allocation, and operating hours to ensure efficiency and quality service delivery during high-demand periods.
  - Positive reviews from elite users and high user engagement can boost a business's online visibility and reputation. Maintaining active engagement with customers and responding promptly to feedback is crucial for building credibility and attracting new customers.
  - Collaborating with elite users and leveraging their influence can amplify promotional efforts, increase brand awareness, and drive customer acquisition. Building strong relationships with key stakeholders, including loyal customers, can further strengthen a business's position in the market.
  - Businesses can adjust their operating hours or introduce special promotions to capitalize on the increased demand during peak hours.
  - Less successful businesses may need to focus on strategies to enhance user engagement over time, such as improving service quality, responding to customer feedback.
  - Cities with high success scores presents opportunities for restaurant chains to expand or invest further.


      















