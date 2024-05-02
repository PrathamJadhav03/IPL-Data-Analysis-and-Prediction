# IPL Data Analysis and Prediction

This is a comprehensive data analysis and prediction project on the Indian Premier League (IPL) cricket matches from 2008 to 2022. The project involves cleaning and preprocessing the dataset, performing exploratory data analysis (EDA), creating visualizations, and building a machine learning model to predict the outcome of IPL matches.

## Dataset

The dataset used in this project is obtained from Kaggle and consists of two CSV files:

`IPL_Matches_2008_2022.csv`: Contains match-level information such as teams, venues, winners, and player of the match.

`IPL_Ball_by_Ball_2008_2022.csv`: Contains ball-by-ball details of each match, including runs scored, wickets taken, and other events.

## Code Walkthrough

The code is divided into several sections, each addressing a specific task. Here's a detailed breakdown of the code:

### 1. Data Loading and Cleaning

The first step is to load the necessary libraries and the two CSV files. The code then performs data cleaning operations, such as handling missing values, renaming teams, converting data types, and eliminating irrelevant matches.

### 2. Creating Batsman and Bowler Statistics

The code creates separate dataframes for batsman and bowler statistics by grouping the ball-by-ball data and computing various metrics like runs scored, balls faced, wickets taken, and strike rates.

### 3. Combining Player Statistics

The code then merges the batsman, bowler, and catch statistics into a single dataframe called final_df. This dataframe contains comprehensive information about each player's performance across different aspects of the game.

### 4. Exploratory Data Analysis (EDA)

The EDA section involves creating various visualizations to gain insights into the data. These visualizations include:

* Bar charts to display the total runs scored, wickets taken, and player of the match awards for each player.
* Scatter plots to identify the best players based on strike rate, catches, bowling economy, sixes, and fours.
* Scatter plots to identify underperforming players based on the number of zeros scored and times out.

### 5. Top Player Identification

The code uses K-Means clustering to identify the top players based on their performance metrics. It creates four clusters of players and presents the players in each cluster.

### 6. Prediction Model Building
The final section of the code focuses on building a machine learning model to predict the outcome of IPL matches. It involves the following steps:

* Data preprocessing: Merging match and ball-by-ball data, handling team name changes, and creating relevant features.
* Feature engineering: Adding features like current score, runs left, balls left, wickets left, current run rate, and required run rate.
* Model training: Using a Random Forest Classifier and a one-hot encoder to train the model on the preprocessed data.
* Model evaluation: Splitting the data into training and testing sets, making predictions on the test set, and evaluating the model's performance.

The code also includes an example of how to use the trained model to predict the outcome of a hypothetical IPL match scenario.

## Usage

To run this code, you'll need to have the following libraries installed:

* pandas
* numpy
* matplotlib
* seaborn
* plotly
* scikit-learn

Additionally, you'll need to download the `IPL_Matches_2008_2022.csv` and `IPL_Ball_by_Ball_2008_2022.csv` files from the provided link and place them in the same directory as your Python script.

## Contributions

Contributions to this project are welcome! If you find any bugs, have suggestions for improvements, or want to add new features, please feel free to open an issue or submit a pull request.