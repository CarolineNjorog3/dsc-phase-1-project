# <span style="color: orange;">  Microsoft's Movie Studio Exploration : From Data Driven To Silver Screen.</span>
**Author** : [Caroline Njeri Njoroge](mailto: njericarol96@gmail.com)
## Project Overview
In a rapidly evolving entertainment landscape, Microsoft is embarking on a bold venture by establishing a new movie studio. The success of this venture hinges on understanding the intricate nuances of the film industry, from market trends to audience preferences. The primary objective of this project is to analyze and leverage movie data effectively to inform decision-making at Microsoft's movie studio. 

### Business Problem
The business problem at hand revolves around Microsoft's venture into the entertainment industry by establishing a new movie studio.
Microsoft faces several challenges and the pain points in this venture, include:
* Understanding Market Dynamics.
* Audience Preferences.
* Financial Success.
* Optimal Release Timing.
* Highly Rated and Popular Movies.
* Language Diversity.
* Budget vs Performance.
By addressing these questions, Microsoft will be better equipped to navigate the complexities of the film industry, produce successful movies, and maximize profitability while providing an enriching cinematic experience to their audience.

### Data Understanding.
The data used for this project were collected from various reputable sources:
* Box Office Performance: Records of box office earnings for a range of movies.
* Genre Trends: Data on the popularity and trending genres over time.
* Audience Preference: Information about the number of people who voted.
* Market Opportunities: Insights into emerging market niches and potential partnerships.
The datasets cover thousands of movies, providing a substantial and diverse sample. The time period covered varies across datasets, with information spanning from historical records to more recent data.
The variables used in this analysis have diverse properties, including numerical, categorical, and ordinal data. Some of the key variables include:
* Movie Title: The title of each film.
* Genre: The genre(s) of the movie.
* Release Date: The date when the movie was released.
* Audience Preference Language: Variables describing the languages the audience prefers.
* Critical Reception: Variables related to ratings and popularity.
* Market Opportunities: Variables associated with emerging market trends and partnership possibilities.
These properties are critical for understanding and analyzing the dataset effectively and for addressing the data analysis questions. This information is essential for framing the context and scope of the subsequent data analysis.

### Data Preparation.
In the process of data preparation, several variables were handled to ensure the dataset's suitability for analysis:
#### Variables Handling:
** Dropping Non-Significant Columns: In the 'tmdbmovies' dataset, we removed non-significant columns ('Unnamed: 0' and 'title') using the drop() method. These columns were irrelevant to the specific analysis questions. This choice was appropriate to streamline the dataset and eliminate unnecessary data that wouldn't contribute to the analysis.

** Cleaning Financial Data: In the 'moviebudget' dataset, we addressed missing values and ensured consistency in the format of financial data. Specifically:

** Removing Commas and Dollar Signs: We removed commas and dollar signs from columns ('production_budget,' 'domestic_gross,' and 'worldwide_gross') to make these values suitable for financial calculations. This was essential to ensure the data's integrity and consistency.
** Converting 'release_date' to Datetime Format: We converted the 'release_date' column to a datetime format using the pd.to_datetime() function. This was crucial to standardize the date format for analysis.
#### Handling Missing Values:
To address missing values, the following steps were taken:

** Dropping Rows with Missing Values: In the 'boxmovies' dataset, rows with missing values in the 'domestic_gross' and 'foreign_gross' columns were removed using the dropna() method. This step ensured that complete financial data was available for analysis.
**Dropping Rows with Missing Studio Information: In the 'boxmovies' dataset, rows with missing values in the 'studio' column were removed to guarantee information about movie studios was available.
** Resetting Index: After removing rows with missing values, the index of the DataFrame was reset using the reset_index() method to maintain data integrity.
** Handling Missing Data in IMDb Dataframes: No specific steps for handling missing data in IMDb-related datasets were mentioned. Depending on the nature and extent of missing data, additional data cleaning and preprocessing could be performed as needed.

