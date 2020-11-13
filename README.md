# Predicting Cancellations on Hotel Reservations
![hotel](https://www.thehotelguru.com/_images/f0/30/f030e43b7ede4f4bc74c7332ae2d3711/portugal-s1180x560.jpg)
<sub><sup>Image Credit: thehotelguru.com</sup></sub>


Cancellations are a massive problem for hotel owners. Especially when they are at the last minute and they do not have time to rebook the room. In our dataset, we have over 100,000 reservations across three years (2015-2017) from two hotels in Portugal. One location lost over €10 million ($11.81 million) in one year. 

Additionally, hotels and the travel industry as whole have been hit hard by the Covid-19 pandemic. However, with Pfizer announcing its new vaccine it will be more important than ever to maximize their profits in 2021 and get back on their feet. To do this, we analyze how the hotels were losing reservations Pre-COVID and create a model to predict which reservations are more likely to be canceled. 

Our model is also optimized to avoid false positives, or predicting a customer will cancel when they do not. With this in mind, hotels can overbook rooms, maximize their profit and avoid a decline in customer satisfaction. 

However, we did find that models oriented for maximising the avoidance of false positives does lead to a dip in profit as then the model is reluctant to predict cancellations. As such, while a Random Forest model that scores a 0.99 precision score (which is a measure of how likely it is to produce True positives) is possible we are recommending our XG boost model which still scores a .9 in precision but is much more accurate. If a hotel is completely risk averse they can use the first model and take a dip in potential profits: we call this the profit-precision trade off. 

By creating a model which accurately predicts cancellations, hotels can maximize their profits by overbooking with confidence. 
![Revenue Loss](https://github.com/acoco10/Hotel-Cancellation-Model/blob/main/images/Revenue_Loss_per_Year.png)

