# Airbnb Data Analysis Dashboard

## As a BI Analyst, I aim to provide a comprehensive, user-friendly interface that integrates various data sources, delivering actionable insights that align with the company's objectives and drive continuous improvement.

## About Dataset
##### New York City Airbnb Data Cleaning

Airbnb, Inc is an American company that operates an online marketplace for lodging, primarily homestays for vacation rentals, and tourism activities. Based in San Francisco, California, the platform is accessible via website and mobile app. Airbnb does not own any of the listed properties; instead, it profits by receiving commission from each booking. The company was founded in 2008. Airbnb is a shortened version of its original name, AirBedandBreakfast.com.

##### Context

Since 2008, guests and hosts have used Airbnb to travel in a more unique, personalized way. As part of the Airbnb Inside initiative, this dataset describes the listing activity of homestays in New York City.

##### Content

The following Airbnb activity is included in this New York dataset:

- Listings, including full descriptions and average review score
- Reviews, including unique ID for each reviewer and detailed comments
- Calendar, including listing ID and the price and availability for that day

## Data Processing and Visualization

First, I cleaned the data using Python and handled missing values. Then, through Python, I connected to the PostgreSQL database, created tables there, and then in Power BI I connected to the PostgreSQL database and created a Dashboard.

## Main Page

The main page features filters and primary visualizations that provide an overview of the data. In addition to the visualizations, there are cards displaying key metrics.

### Filters

- Cancellation Policy
- Neighborhood
- Room Type
- Availability (0 to 365 days)
- Price ($50 to $1200)

### Key Metrics

- Total Reviews: 3M
- Total Houses: 102.06K
- Average Reviews per Month: 1.16

### Visualizations

- **Average Price by Neighborhood:** A bar chart showing the average prices in various neighborhoods.
- **Total Neighborhoods by Group:** A pie chart displaying the distribution of neighborhoods by group (Manhattan, Queens, Staten Island, Bronx, Brooklyn).
- **Top 10 Houses by Total Reviews:** A bar chart listing the top 10 houses based on the number of reviews.
- **Total Listings by Neighborhood and Room Type:** A bar chart showing the distribution of listings by neighborhood and room type (Entire home/apt, Hotel room, Private room, Shared room).
- **Average Price by Neighborhood Group and Room Type:** A table showing average prices by neighborhood group and room type.
- **Total Houses by Construction Year:** A bar chart showing the total number of houses built per year.

![Main Page](https://github.com/user-attachments/assets/5e76a76c-e5b0-4c44-8a81-8b5b5f2d6b84)

## Listings Page

The listings page includes filters, a table, and a map. The size of the bubbles on the map represents the average house price at that location.

### Filters

- Neighborhood
- Room Type
- Number of Reviews (slider from 0 to 1024)
- Price ($50 to $1200)

### Visualizations

- **Map:** Displays bubbles representing the average house price at different locations. The size of the bubble correlates with the price.
- **Table:** Shows detailed information about the listings, including ID, Name, Host Name, Host ID, Price, Minimum Nights, Availability, Review Rate Number, and Last Review.

![Listings Page](https://github.com/user-attachments/assets/f1559115-bc14-4229-84f6-038abea0528d)

When a bubble is clicked, the table displays detailed information about the corresponding listing. Additionally, hovering over a bubble reveals information for that data point through a tooltip.

- **Tooltip:** Provides information about the listing when hovering over a bubble on the map.

![Tooltip](https://github.com/user-attachments/assets/1adfe1bf-6b0f-4ffb-97a2-a49d6d55324e)

## Neighborhoods Page

The Neighborhoods Page features multiple visualizations and insights into the performance of various neighborhoods in the Airbnb market.

### Visualizations

- **Top 5 by Average Price:** This chart shows the top 5 neighborhoods based on the average price and rating. It highlights the relationship between price and guest ratings.
- **Top 5 by Average Review:** This bar chart displays the top 5 neighborhoods with the highest average review scores, helping to identify areas with the best guest feedback.
- **Top 10 with Most Listings:** A bar chart illustrating the top 10 neighborhoods with the highest number of listings, indicating the most popular areas for Airbnb properties.
- **Availability across Neighborhoods:** This chart shows the availability of listings across different neighborhoods, providing insights into the supply of Airbnb properties in each area.

This dashboard offers a comprehensive overview of key metrics and trends across various neighborhoods, aiding in decision-making and strategic planning.

![Neighborhoods Page](https://github.com/user-attachments/assets/92578c64-546f-4701-bd0b-07ed307c5e97)

## KPI Page

The KPI page features filters, key metrics, and a line chart, providing insights into the financial performance and review trends of the listings.

### Filters

- Cancellation Policy
- Neighborhood
- Room Type
- Availability (0 to 365 days)
- Price ($50 to $1200)

### Key Metrics

- Average Revenue per Listing: $7.72K
- RevPAL (Revenue per Available Listing): $79.71K
- Average Price per Night: $625

### Visualization

- **Total Last Review by Year:** A line chart displaying the total number of last reviews by year, highlighting trends over time. The chart shows significant peaks in the years 2019 and 2020.

![KPI Page](https://github.com/user-attachments/assets/b38bc158-4dc1-42c3-b99a-376f9a860eac)

When you hover over each bar, a tooltip appears, explaining the KPI and showing a detailed chart of KPI for each neighborhood group. This feature is created using the tooltip functionality.

- **Tooltip:** Provides information about the KPI when hovering over a card.

![Tooltip](https://github.com/user-attachments/assets/fc60c134-3b39-4a31-b4e8-b114cbdce0f1)

## Getting Started

### Prerequisites

- [Python 3.x](https://www.python.org/downloads/)
- [Jupyter Notebook](https://jupyter.org/install)
- [Power BI Desktop](https://powerbi.microsoft.com/desktop/)
- Required Python packages (listed in `requirements.txt`)

### Installation

