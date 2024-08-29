# Candy Recommender System

## Project Overview
The Candy Recommender System is designed to predict an individual's candy preferences based on their taste profile. The project utilizes machine learning techniques, including clustering and recommendation algorithms, to analyze a dataset of 85 different candies and their attributes.

## Data Understanding & Visualization
The dataset includes the following features:
- **chocolate**: Contains chocolate or not.
- **fruity**: Fruit-flavored or not.
- **caramel**: Presence of caramel.
- **peanutyalmondy**: Contains peanuts, peanut butter, or almonds.
- **nougat**: Presence of nougat.
- **crispedricewafer**: Contains crisped rice wafers or cookie component.
- **hard**: Hard candy or not.
- **bar**: Candy bar or not.
- **pluribus**: One of many candies in a bag or box.
- **sugarpercent**: Sugar content percentile.
- **pricepercent**: Price percentile.
- **winpercent**: Popularity measure based on vote percentage.

### Visualizations
- **Correlation Matrix**: A heatmap was generated to visualize the correlations between different features in the dataset.
- **Pairplot**: Used for exploring the relationships between features.

## Preprocessing
- Checked for null values and found none.
- Removed duplicates, resulting in a dataset with 85 entries and 13 features.

## Experiment 1: Clustering and PCA
### Modeling
- **Feature Selection**: Selected 9 features related to candy attributes for clustering.
- **Standardization**: Applied `StandardScaler` to standardize the features.
- **Principal Component Analysis (PCA)**: Reduced the dataset to 2 principal components, explaining approximately 61.19% of the variance.
  
### Clustering
- **K-Means Clustering**: Tested various numbers of clusters using the Silhouette Method. The optimal number of clusters was determined to be 4.

### Visualization
- **Scatter Plot**: Visualized the clusters using the two principal components.

## Experiment 2: Recommender Systems
- **Cosine Similarity**: Calculated the cosine similarity between candies based on their attributes to recommend similar candies.
- **Recommendation Function**: A function was implemented to recommend candies similar to a given candy.

### Example Recommendation
Recommending 5 candies similar to "Nestle Crunch":
- Kit Kat
- Nestle Crunch
- 100 Grand
- Twix
- Tootsie Roll Snack Bars

## Evaluation
- **Root Mean Square Error (RMSE)**: The model's performance was evaluated using RMSE, which was calculated to be approximately 0.228.

## Insights
- **Clustering**: Clear distinctions between candy types were identified, making the clustering model effective.
- **Recommendations**: The recommender system successfully identified similar candies based on taste profiles.

## Impact
- **Positive**: Helps users discover new candies they might enjoy, provides personalized recommendations, and can promote health awareness by suggesting lower-sugar options.
- **Negative**: Could increase sugar consumption, especially among children.

## Contributors
- Pranav ytDadu
- Yojith Mandapati
- Thien Nguyen
- Kegan Edwards
- Ninh Nguyen

