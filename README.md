# How can we help Hotels maximize their available rooms?

Cancellations are a massive problem for hotel owners. Especially when they are at the last minute and they do not have time to rebook the room. In our dataset that includes over 100,000 reservations over three years (2015-2018) at two hotels in Portugal, one location lost over a million euros one year. By creating a model which accurately predicts cancellations, hotels can maximise their profits by overbooking with confidence. Hotels and the travel industry as whole have been hit hard by the Covid-19 pandemic. With Pfizer announcing its new vaccine it will be more important than ever to maximise their profits in 2021 and get back on their feet. Our model is also optimized to avoid false positives, or predicting a customer will cancel who does not, with this in mind hotels can overbook rooms, maximise their profit and avoid a decline in customer satisfaction. However, we did find that models oriented for maximising the avoidance of false positives does lead to a dip in profit as then the model is reluctant to predict cancellations. As such while a random forest model that scores a .99 precision score (which is a measure of how likely it is to produce false positives) is possible we are recommending our XG boost model which still scores a .9 in precision but is much more accurate. If a hotel is completely risk averse they can use the first model and take a dip in potential profits: we call this the profit-precision trade off. 

