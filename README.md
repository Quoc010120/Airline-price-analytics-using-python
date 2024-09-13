![airplane](/img/background1.jpg)

# AIRLINES PRICE ANALYTICS

## Introduction

In this project, I will work for a travel agency and aim to understand airline prices thoroughly to assist clients in finding the best deals. My goal is to analyze how airline prices fluctuate based on various factors. The main sections of this research include defining the questions, data preparation, data analysis, and conclusions.

The project aims to answer the following questions:

- What is the average coach price, and is \$500 a reasonable price for a coach ticket?
- How do flight hours affect coach ticket prices, specifically for an 8-hour flight?
- What types of delays are most common, and how do they affect connecting flights?
- What is the relationship between coach prices and other flight features?

**Data Sources:**
The dataset `flight.csv` was provided by Codecademy.com.

![dog-funny](/img/background2.jpg)

## Data

This project uses a single dataset, a CSV file containing information about "My Favorite Airline." The data will be analyzed to address the research questions.

_Note: The data used is inspired by real-world data but primarily fictional._

The dataset includes:

- `miles`: miles traveled during the flight
- `passengers`: number of passengers on the flight
- `delay`: take-off delay in minutes
- `inflight_meal`: whether a meal is included
- `inflight_entertainment`: availability of entertainment systems
- `inflight_wifi`: availability of complimentary Wi-Fi
- `day_of_week`: day of the flight
- `weekend`: whether the flight took place on a weekend
- `coach_price`: average price paid for a coach ticket
- `firstclass_price`: average price paid for first-class seats
- `hours`: flight duration in hours
- `redeye`: whether the flight is a redeye

## Analytics

### Coach Price Distribution

The first question is, "What is the average coach price, and is \$500 a reasonable price for a coach ticket?" To answer this, we will create a box plot.

Based on the box plot (Figure 1), coach ticket prices range from \$100 to \$500. The highest outlier is \$600, and the lowest is \$0. The first quartile (Q1) is \$190, and the average coach price is \$376, indicating that \$500 seems a bit high for a coach ticket.

To have a clearer view of coach price distribution, we look at Figure 2, which shows the histogram of coach prices centered between \$350 and \$400.

![boxplot-coach-price](/img/figure1.png)

![hist-coach-price](/img/figure2.png)

### Coach Ticket Prices for 8-Hour Flights

Next, we focus on visualizing coach ticket prices for 8-hour flights to understand the distribution and whether a \$500 ticket is more reasonable for such flights.

#### Visualization and Analysis

The box plot and histogram for 8-hour flights reveal:

- **High Price:** \$580
- **Low Price:** \$120
- **Average Price:** \$410

Compared to the overall average coach price (\$376), prices for 8-hour flights are higher, making a \$500 ticket more reasonable in this context.

![8-hours-flight-coach-price](/img/figure3.png)

### Distribution of Flight Delay Times

This section explores flight delay times to better understand their impact on connecting flights.

#### Visualization and Analysis

Figure 3 shows that most delays are between 5 and 15 minutes, with a significant peak at 10 minutes. Longer delays, though less common, extend up to 50 minutes.

![hist-number-delay-time](/img/figure4.png)

#### Implications for Connecting Flights

Given this distribution, most flights experience short delays, but longer delays do occur. Clients should schedule connecting flights with enough buffer time to avoid missed connections.

### Relationship Between Coach and First-Class Prices

A scatter plot with a trend line (Figure 4) shows a positive correlation between coach and first-class prices: as coach prices rise, first-class prices also increase, though not perfectly linearly.

![scatter-coach-price-first-class](/img/figure5.png)

### Relationship Between Coach Prices and Inflight Features

This section examines how inflight features affect coach prices.

#### Inflight Meals

Flights with meals have slightly higher prices, though the overall distribution is similar to flights without meals.

![coach-price-inflight-meal](/img/figure6.png)

#### Inflight Entertainment

Flights with entertainment are generally more expensive, as shown by a shift towards higher prices.

![coach-price-inflight-enter](/img/figure7.png)

#### Inflight WiFi

Flights with WiFi access are also priced higher, reflecting the added value of internet connectivity.

![coach-price-inflight-wf](/img/figure8.png)

### Relationship Between Number of Passengers and Flight Hours

The scatter plot shows that short flights (1 to 5 hours) have a relatively stable number of passengers, while longer flights (6 to 8 hours) tend to have fewer passengers, possibly due to comfort and convenience preferences.

![number-passenger-flight-hours](/img/figure9.png)

### First-Class Price Differences on Weekends

The graph shows that both coach and first-class prices are generally higher on weekends compared to weekdays, indicating that airlines adjust pricing based on travel demand.

![coach-price-first-class-in-weekend](/img/figure10.png)

### Analysis of Coach Prices for Redeye and Non-Redeye Flights

A box plot compares coach prices for redeye and non-redeye flights across the week:

- **Weekdays:** Redeye flights generally have lower prices than non-redeye flights.
- **Weekends:** Both types of flights have higher prices on weekends, with non-redeye flights still being slightly more expensive.

![coach-price-and-redeyes](/img/figure11.png)
