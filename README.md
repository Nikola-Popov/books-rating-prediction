# Training a prediction model for the average rating of a book
---
### Motivation
This project will serve as an item based recommendation system for the average rating of a book. Thus no new user preferences will be taken into account. We will solely rely on the already rated books.

### Data source
The dataset is a sample from Goodreads.com and is published at: https://www.kaggle.com/jealousleopard/goodreadsbooks

### Results overview
From the observations we see that a _GradientBoostingRegressor_ with preprocessed data (using polynoms of 2nd degree) performed the best on the test data with score like ~19%. On the training data it did good - around 53%. However the overall scores are not very good but the actual vs. predicted data printed displays some satisfying results. This random sample table looks like this:

| Actual  | Predicted  |
|---|---|
|4.28  | 4.205785 |
| 3.68  | 3.859051 |
| 3.91  | 3.927412 |
| 3.78  | 3.904838 |
| 3.97  | 3.906189 |
| 3.89  | 3.844968 |
| 3.68  | 3.971978 |
| 3.26  | 3.885882 |
| 3.82  | 3.722159 |
| 4.19  | 3.986447 |

### Dumped model
books_model.pkl contains the serialized that best fit the training and the testing data.
