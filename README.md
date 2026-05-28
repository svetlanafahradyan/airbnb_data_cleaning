# airbnb_data_cleaning

![airbnb listing dataset](https://mohamedirfansh.github.io/Airbnb-Data-Science-Project/images/seattle.jpg)


## Resources 
[Kaggle Dataset](https://www.kaggle.com/datasets/arianazmoudeh/airbnbopendata)


## Project Sturcture 

```
├── Airbnb_Open_Data.csv       # Raw source data 
├── clean_airbnb_data.csv      # Cleaned dataset
├── data_cleaning.ipynb        # Main notebook
├── .gitignore                 
└── README.md
```


## Dependencies
- pandas
- numpy
- matplotlib
- seaborn
- jupyter


## Cleaning Steps

| Step | Description |
| ----------- | ----------- |
| Inspection | Shape, dtypes, null counts, duplicates |
| Duplicates | Drop exact duplicate rows |
| Text cleaning | Strip whitespace, lowercase categoricals |
| Fix inconsistencies | standardize capitalization, fix typos, unify category names |
| Missing values | Drop / impute based on column type and % missing |
| Type conversion | Fix dtypes: prices → float, dates → datetime, etc. |
| Export | Save to clean_airbnb_data.csv |


## 📋 Columns

| Original Column | Cleaned Column |
|-----------------|----------------|
| `id` | `listing_id` |
| `NAME` | `listing_name` |
| `host id` | `host_id` |
| `host_identity_verified` | `host_identity_verified` |
| `host name` | `host_name` |
| `neighbourhood group` | `borough` |
| `neighbourhood` | `neighbourhood` |
| `lat` | `latitude` |
| `long` | `longitude` |
| `country` | `country` |
| `country code` | `country_code` |
| `instant_bookable` | `instant_bookable` |
| `cancellation_policy` | `cancellation_policy` |
| `room type` | `room_type` |
| `Construction year` | `construction_year` |
| `price` | `price` |
| `service fee` | `service_fee` |
| `minimum nights` | `min_nights` |
| `number of reviews` | `review_count` |
| `last review` | `last_review_date` |
| `reviews per month` | `reviews_per_month` |
| `review rate number` | `review_rating` |
| `calculated host listings count` | `host_listing_count` |
| `availability 365` | `availability_days_per_year` |
| `house_rules` | `house_rules` |
| `license` | `license_number` |


## Output
The cleaned dataset clean_airbnb_data.csv has:

- No duplicate rows
- Consistent data types across all columns
- Missing values handled or flagged
- Ready for EDA, visualization, or ML modeling
