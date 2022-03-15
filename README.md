# SageMaker Data Wrangler L400 Workshop



**Use Case**

* Predicting hotel booking cancelations

**Dataset**

* [Hotel Booking Demand dataset](https://www.kaggle.com/jessemostipak/hotel-booking-demand) - This data set contains booking information for a city hotel and a resort hotel, and includes information such as when the booking was made, length of stay, the number of adults, children, and/or babies, and the number of available parking spaces, among other things.
![Hotel Booking](./img/hotel-booking.png)

**Description of the columns**

| Column Name  | Description  | 
|---|---|
| `hotel`  | Type of the hotel (H1 = Resort Hotel or H2 = City Hotel)  |   
| `is_canceled` | Value indicating if the booking was canceled (1) or not (0) |   
| `lead_time` | Number of days that elapsed between the entering date of the booking into the PMS and the arrival date |
| `arrival_date_year` | Year of arrival date |
| `arrival_date_month` | Month of arrival date |
| `arrival_date_week_number` | Week number of year for arrival date |
| `arrival_date_day_of_month` | Day of arrival date |
| `stays_in_weekend_nights` | Number of weekend nights (Saturday or Sunday) the guest stayed or booked to stay at the hotel |
| `stays_in_week_nights` | Number of week nights (Monday to Friday) the guest stayed or booked to stay at the hotel |
| `adults` | Number of adults |
| `children` | Number of children |
| `babies` | Number of babies |
| `meal` | Type of meal booked. Categories are presented in standard hospitality meal packages: Undefined/SC – no meal package; BB – Bed & Breakfast; HB – Half board (breakfast and one other meal – usually dinner); FB – Full board (breakfast, lunch and dinner) |
| `country`| Country of origin. Categories are represented in the ISO 3155–3:2013 format |
|`market_segment`|Market segment designation. In categories, the term “TA” means “Travel Agents” and “TO” means “Tour Operators”|
|`distribution_channel`|Booking distribution channel. The term “TA” means “Travel Agents” and “TO” means “Tour Operators”|
|`is_repeated_guest`|Value indicating if the booking name was from a repeated guest (1) or not (0)|
|`previous_cancellations`|Number of previous bookings that were cancelled by the customer prior to the current booking|





**Exploratory Data Analysis**
TODO

**Feature Transformations**
TODO

**Evaluate Feature importance**
* Which features are most important to predict cancelations?


TODO

