## Data Transformations 



 ### Drop Columns 
 drop columns based on the analyses we performed in the previous section. 
 
 
 based on target leakage
 
 drop `reservation_status`
 
 drop 7 columns that are redundant - `days_in_waiting_list`, `hotel`, `reserved_room_type`, `arrival_date_month`, `reservation_status_date`, `babies` and `arrival_date_day_of_month`
 
 
 
 based on linear correlation results 
 
 `arrival_date_week_number`
 `arrival_date_year` is greater than the recommended threshold of `0.90`
 
 
 based on non-linear correlation results
 we need to drop `reservation_status`
 
we had already dropped it since it was also a target leakage 

 






### Balancing the target variable 

`is_canceled` = 0 (negative case)
`is_canceled` = 1 (positive case)

The ratio of positive to negative case = 23589/62440 = ~0.38

Balance using SMOTE







### Quick Model 
![quick-model-post](.././img/quick-model-post.png)

