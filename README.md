# surfs_up
## OVERVIEW
In this project, we are extracting year-over-year temperature trends by month from a SQLite local database.
### PURPOSE
The purpose of the project is to analyze seasonal trends in climate to project potential economic impact on a new business venture in a locale whose given spending population is greatly affected by tourism.
## RESULTS
The seasonal difference experienced in most climates and previously assumed to have significant effect might be, in fact, insignificant enough to mostly ignore--to the delight of the business partners in the project.
### WEATHER DIFFERENCES B/W JUNE AND DECEMBER
1. More temperatures were collected for June than December due to the fact that 2017's December data hasn't yet been collected, so we have an extra year for the summer month's veracity.
2. The difference in temperature is largely negligible, with it being colder at most data points in the winter months--most notably at the lower quartile.
3. The standard deviation of the December data is larger, meaning the fluctuation in temperature is larger and the predictability of the weather from day to day isn't as high.
## SUMMARY
What might have been an understandably expected seasonal difference is largely insignificant compared to the difference experienced in most more-temperate climates than the Hawaiian tropic of Oahu. It is largely a near-perfect surfing hotspot year round, meaning that business ought to see a largely consistent set of trafficking tourists to help fuel its cashflow.
### ADDITIONAL QUERIES
The below two queries will provide additional weather data in the form of year-over-year seasonal trends in precipitation pattern.
1. session.query(Measurement.prcp).filter(extract('month', Measurement.date) == 6).all()
2. session.query(Measurement.prcp).filter(extract('month', Measurement.date) == 12).all()
