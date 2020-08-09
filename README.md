# Airbnb-Seattle
![ AirBnB](https://productcharles.com/wp-content/uploads/2015/11/airbnb_logo_detail.png)

**Airbnb reservation price is based on following costs (according to [Airbnb official website information](https://www.airbnb.co.in/help/article/125/how-is-the-price-determined-for-my-reservation?locale=en&_set_bev_on_new_domain=1593369098_ODJmM2Y0YjZlNjhl)):**

- **Costs determined by the host:**
  - **Nightly price:** Nightly rate decided by the host;
  - **Cleaning fee:** One-time fee charged by some hosts to cover the cost of cleaning their space;
  - **Extra guest fee:** Fee charged by some hosts for each guest beyond a set number;
- **Costs determined by Airbnb:** Airbnb service fee;
- **Other costs that may be included:** currency exchange fees, VAT, other local taxes etc

In our analysis we will concentrate on the factors, which influence the nightly price, determined by the host. Actually, Airbnb already has an algorithm, which suggests hosts the price. The approach for the algorithm and challenges are described in the article [here](https://www.vrmintel.com/inside-airbnbs-algorithm/). We can also use the information from the article in our analysis.

- Time of the year, when reservation is made, affects the price;
- Amenities offered like Wi-Fi and TV should be considered in the analysis, as they also might have great influence on price;
- It is better to use neighbourhood information rather then exact coordinates to describe the listing location, because sometimes even close locations might have huge difference in listing prices, if they belong to different neighbourhoods or are located different sides of the river.

## Motivation
- What is the seasonal pattern of Airbnb in Seattle?
- What are the busiest times of the year to visit Seattle? 
- How does rental pricing increase or decrease by season and what is the peak season in Seattle?
- What is the most expensive weekday and month ?
- How does pricing increase or decrease by neighborhood and which ones are the priciest neighborhoods in Seattle?
- What are the most influential features about the rental price?

AirBnB provided us with 3 datasets for Seattle:

- **listings.csv** - summary information on listing in Seattle such as: location, host information, cleaning and guest fees, amenities etc.
- **calendar.csv** - calendar data for the listings: availability dates, price for each date.
- **reviews.csv** - summary review data for the listings.
