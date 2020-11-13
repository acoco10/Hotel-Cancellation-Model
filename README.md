# Predicting Cancellations on Hotel Reservations
![hotel](https://www.thehotelguru.com/_images/f0/30/f030e43b7ede4f4bc74c7332ae2d3711/portugal-s1180x560.jpg)
<sub><sup>Image Credit: thehotelguru.com</sup></sub>


Cancellations are a massive problem for hotel owners. Especially when they are at the last minute and they do not have time to rebook the room. In our dataset, we have over 100,000 reservations across three years (2015-2017) from two hotels in Portugal. One location lost over €10 million ($11.81 million) in one year. 

Additionally, hotels and the travel industry as whole have been hit hard by the Covid-19 pandemic. However, with Pfizer announcing its new vaccine it will be more important than ever to maximize their profits in 2021 and get back on their feet. To do this, we analyze how the hotels were losing reservations Pre-COVID and create a model to predict which reservations are more likely to be canceled. 

Our model is also optimized to decrease false positives (predicting a customer will cancel when in reality they do not cancel). By creating a model which predicts cancellations precisely, hotels can maximize their profits by overbooking with confidence. 

However, we did find that models oriented for maximising the avoidance of false positives does lead to a dip in profit as then the model is reluctant to predict cancellations. As such, while a Random Forest model that scores a 0.99 precision score (which is a measure of how likely it is to produce True positives) is possible we are recommending our XG boost model which still scores a .9 in precision but is much more accurate. If a hotel is completely risk averse they can use the first model and take a dip in potential profits: we call this the profit-precision trade off. 


## Data:
Data was acquired from a research by [Antonio, Almeida and Nunes, 2019.](https://www.sciencedirect.com/science/article/pii/S2352340918315191?via%3Dihub) for Revenue Management, data analysis and Machine Learning. The dataset we worked with was cleaned by and provided by [Tidy Tuesday](https://github.com/rfordatascience/tidytuesday/blob/master/data/2020/2020-02-11/readme.md). 
It consists of 119390 observations (Hotel Reservations with guest information) and 32 features. 

## Discovery:

The overall we see there are more reservations and cancellations at the "City Hotel" when compared to the "Resort Hotel". 
Although the Average Daily Rate (adr) is higher at the "City Hotel" (€105.30) comapred to the "Resort Hotel' (€94.95), people tend to stay longer at the resort with average total nights of 4.32 nights and 2.98 nights at the city hotel. 

![

![Revenue Loss](https://github.com/acoco10/Hotel-Cancellation-Model/blob/main/images/Revenue_Loss_per_Year.png)

