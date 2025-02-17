# Book-Recommendation-System
A well developed recommendation system will help businesses improve their shopper's experiences on their websites and result in better customer acquisition and retention.
The recommendation system, I have designed below is based on the journey of a new customer from the time he/she lands on the business’s website for the first time to when he/she makes repeat purchases.
I designed the recommendation system in three parts:
Recommendation system part I: Product popularity based.
Recommendation system part II: Model-Based Collaborative Filtering System
Recommendation system part III: Search engine based

I used [Amazon Book review](https://www.kaggle.com/datasets/mohamedbakhet/amazon-books-reviews?select=Books_rating.csv) Dataset for this project. It consists of two data sets: Books_rating and books_data. The books rating dataset contains the book id, book name, rating, etc. And the books data consists of the book title, author, description, category, etc,. So I combined and processed the data together such that it fits my requirements.

## Recommendation System Part I
Popularity based are a great strategy to target the new customers with the most popular products sold on a business's website and is very useful to cold-start a recommendation engine.
## Recommendation System Part II
* Recommend books to users based on purchase history and similarity of ratings provided by other users who bought items to that of a particular customer.
* A model based collaborative filtering technique is closen here as it helps in predicting books for a particular user by identifying patterns based on preferences from multiple user data.
An utlity matrix consisting of all possible user-item preferences (ratings) details is generated. The utility matrix is sparce as none of the users would buy all the items in the list, hence, most of the values are unknown.
A decomposition and correlation matrix is created. Correlation of all books with the book purchased by this customer based on items rated by other customers who bought the same book.
Thereby based on a previous purchase, collaborative filtering is done and top 10 books are recommended.
## Recommendation System Part III
For a business without any book purchase history, a search engine based recommendation system is designed. The book recommendations can be based on the textual clustering analysis given in book description.
Converted the text in product description into numerical data for analysis using TfidfVectorizer, followed by the implementation of the Kmeans clustering model.
