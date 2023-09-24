# **Project Name**

### **Exploratory Data Analysis - Airbnb Booking**

#### Programming language: Python
#### Libraries used: Numpy, Pandas, Matplotlib, Seaborn 
#### NoteBook: Google Colab
#### Dataset Source: Provided by AlmaBetter


## **Project Summary-**

Airbnb, a global online marketplace for lodging and travel experiences, has revolutionized the way people travel and find accommodations. For both hosts and travelers, Airbnb offers a platform where they can list or book unique properties and experiences in various destinations worldwide. This summary presents an analysis of Airbnb booking data, shedding light on key insights that can inform business strategies, pricing decisions, and customer experiences.


## **Problem Statement-**

The objective of this data analysis project is to extract actionable insights from a comprehensive Airbnb dataset encompassing various attributes such as property details, host information, location, pricing, and booking history. We aim to address key questions, including understanding pricing dynamics based on room types and locations, identifying factors influencing booking demand, and uncovering host-related patterns.


## **Business Objective**

The primary business objective of this Airbnb data analysis project is to empower hosts and travelers with data-driven insights to optimize their experiences on the platform by Optimizing Pricing Strategies based on factors such as location, property type and seasonal demand. Enhancing Guest Satisfaction by identifying commonality in customer reviews and feedback to help hosts improve their offerings and enhance the overall guest experience. Host Profiling based on property portfolios and reviews. This will provide guidance to both current and prospective hosts on achieving most booking conclusions like analysing booking trends, occupancy rates, and availability patterns to help hosts maximize their property occupancy and revenue.


## Dataset

Dataset link - https://drive.google.com/file/d/1ioU5r9KEYSfwgfUi22SclVkx4l1a_8ou/view

Dataset contains information of Airbnb columns:
```
* **id:** This is likely a unique identifier for each accommodation listing.

* **name:** The name or title of the accommodation.

* **host_id:** A unique identifier for the host of the accommodation.

* **host_name:** The name of the host.

* **neighbourhood_group:** The broader geographical group or region within which the accommodation is located (e.g., borough in a city).

* **neighbourhood:** The specific neighborhood or area within the 'neighbourhood_group' where the accommodation is situated.

* **latitude and longitude:** The geographic coordinates of the accommodation.

* **room_type:** The type of room or space being offered (e.g., entire home/apartment, private room, shared room).

* **price:** The cost of renting the accommodation.

* **minimum_nights:** The minimum number of nights a guest is required to book when staying at this accommodation.

* **number_of_reviews:** The total number of reviews that have been submitted for this accommodation.

* **last_review:** The date of the last review submitted for this accommodation. 'reviews_per_month': The average number of reviews per month for this accommodation.

* **calculated_host_listings_count:** The total number of listings managed by the host.

* **availability_365:** The number of days the accommodation is available for booking in a year (out of 365 days).
```

- Total number of rows in data: 48895
- Total number of columns: 16

 ## **Data Wrangling**

 **1. Duplicates rows:** As there are 48895 rows and 16 columns in the dataset no duplicates found in the dataset.

 **2. handling cleaning & missing value:**

 **2.1** To replace null values with a specific date (e.g., '0000-00-00') in the 'last_review' column of the DataFrame, you can use the fillna method. However, 
'0000-00-00' is not a valid date, so replace null values with a more appropriate default date (e.g., '1970-01-01') instead of an invalid value.

 **2.2** The "reviews_per_month" column represents number of reviews in a month contains 10,052 null values out of 48,895 which is 10%. By replacing null with 0, the column remains consistent interms of data type(integer) and can be included in data manipulation without issues related to missing data.

 **3. Type casting:**

type casting involves changing the data type of a variable or value from one type to another, it plays a crucial role in data manipulation like data compatibility, data integrity and mathematical operations.

## *Data Vizualization, Storytelling & Experimenting with charts : Understand the relationships between variables**

#### **Univariate Analysis -**
```
Chart - 1 Neighbour hood group counts

Chart - 2 Room type distribution

Chart - 3 Neighbourhood Counts

Chart - 4 Host Listings
```
#### **Bivariate Analysis -**
```
Chart - 5 Latitude and Longitude

Chart - 6 Neighbour hood group mean price

Chart - 7 Room_type in Neighbourhood_group

Chart - 8 Neighbour hood group reviews

Chart - 9 Average month reviews

Chart - 10 Top-3 Neighbourhoods in each Neighbourhood group
```
#### **Multi-variate Analysis -**
```
Chart - 11 Average room price for neighbour hood group

Chart - 12 Correlation Heatmap

Chart - 13 - Pair Plots for various columns
```
## **Solution To Business Objective**

**Optimize Pricing Strategy:** Determine the most profitable pricing strategy for hosts based on factors like room type, neighborhood group, and seasonality.

**Increase Occupancy Rates:** Identify factors affecting occupancy rates and develop strategies to maximize property bookings throughout the year.

**Enhance Guest Experience:** Analyze customer reviews and feedback to understand common issues and improve guest experiences.

**Host Profiling:** Profile hosts based on earnings, property portfolio, and reviews to identify characteristics of successful hosts.

**Market Segmentation:** Segment travelers based on their preferences for room type, neighborhood group, and price range to target specific market segments effectively.

**Demand Forecasting:** Predict booking demand based on historical data, seasonality, and external factors to optimize property availability.

**Competitive Analysis:** Analyze competitor listings in terms of pricing, amenities, and customer satisfaction to stay competitive.

**Property Portfolio Management:** Help hosts make informed decisions about expanding or diversifying their property portfolio.

**Seasonal Trends:** Understand how seasonality impacts booking trends and develop strategies for peak and off-peak seasons.

**Review Response Strategy:** Develop a strategy for hosts to respond to guest reviews and manage their online reputation effectively.

**Predictive Maintenance:** Implement predictive maintenance for property upkeep based on historical data and reviews.

**Market Expansion:** Identify potential neighborhoods or geographical areas for hosts to consider expanding their listings.

## **Conclusion**

**1. Neighbour hood group counts:** The data reveals a clear concentration of listings in Manhattan and Brooklyn, with significantly fewer listings in Bronx and Staten Island. Property owners and businesses should focus their efforts on Manhattan and Brooklyn for Airbnb listings, considering their higher demand and market potential, while also exploring opportunities for growth and competition in these popular areas.

**2. Room type distribution:** The pie chart illustrates the room type distribution, with "Entire home/apt" being the most prevalent at 52.0%, followed by "Private room" at 45.7%, and "Shared room" at 2.4%. This indicates a majority of listings are for entire homes or apartments, while private rooms are also common, and shared rooms represent a smaller segment of the listings.

**3. Neighbourhood counts:** In the dataset, "Williamsburg" stands out as the neighbourhood with the highest number of listings (3920), followed closely by "Bedford-Stuyvesant" (3714). "Harlem" also ranks among the top neighborhoods with 2658 listings, while "Crown Heights" and "Midtown" have relatively fewer listings compared to others.

**4. Host Listings:** In the dataset, it's evident that host "Michael" has the highest number of listings (450), indicating significant activity and experience in hosting. Conversely, hosts like "David" (410 listings) may be relatively less active or new to the platform, while "Alex" (260 listings) has the fewest listings among these hosts, suggesting a lower level of engagement.

**5.Latitude and Longitude:** The scatterplot analysis indicates that Brooklyn has the highest listing density, followed by Manhattan and Queens. Additionally, overlapping dots in specific areas suggest concentrated listings within certain neighborhood groups, revealing variations in property distribution across regions.

**6.Neighbour hood group mean price:** The analysis reveals that Manhattan has the highest average listing price at (USD 196.87), followed by Brooklyn at (USD 124.38). In contrast, the Bronx has the lowest average listing price, standing at (USD 87.49), among the considered neighborhoods. This suggests significant price variations based on location.

**7.Room_type in Neighbourhood_group:** Observations made from plot in Entire home/apt majority neighbourhood groups are "Manhattan" followed by "Brooklyn", whereas in Private room majority neighbourhood groups are "Brooklyn" followed by "Manhattan" and lastly in Shared room type majority is "Manhattan" followed by "Brooklyn".

**8. Neighbour hood group reviews:** The chart reveals that "Queens" and "Manhattan" have the highest numbers of reviews, indicating a higher level of activity and feedback for listings in these neighborhood groups. These areas may attract more visitors and gather more attention from guests, potentially making them attractive locations for hosts and property owners.

**9. Average month reviews:** The chart illustrates fluctuations in the average number of reviews throughout the year, suggesting possible seasonal trends in customer activity. The peak occurs in June and July, with averages of 46.25 and 42.70, respectively, followed by a sharp decline in August. This pattern indicates a higher level of guest engagement during the summer months and a potential decrease in August.

**10.Neighbourhoods in each Neighbourhood group:** The chart illustrates the distribution of listings across various neighborhood groups. "Upper West Side" stands out with the highest count of listings within its group, indicating it is a prominent area for Airbnb listings compared to other neighborhoods in their respective groups.

**11.Average room price for neighbour hood group:** The price variations for different room types within each neighbourhood group. "Manhattan" stands out with the highest average price for "Entire home/apt" at (USD 230.92), followed by 'private room'(USD 109.97) and "shared room" (USD 92.79). "Brooklyn" and "Staten Island" also exhibit varying pricing trends, providing valuable insights for hosts and property owners regarding room type pricing strategies.




