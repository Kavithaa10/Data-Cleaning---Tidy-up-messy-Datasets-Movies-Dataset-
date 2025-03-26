# Data-Cleaning---Tidy-up-messy-Datasets-Movies-Dataset-

## Project Brief

### First Steps

### Dropping irrelevant Columns

### Handle stringified JSON column

### Flatten nested Columns

### Cleaning Numerical Columns

### Cleaning DateTime Columns

### Cleaning Text / String Columns

### Removing Duplicates

### Handling Missing Values & Removing Observations

### Final (Cleaning) Steps



### First Steps
#### 1.	Load and inspect the messy dataset movies_metadata.csv. Identify columns with nested / stringified json data.

### Dropping irrelevant Columns

#### 2.	Drop the irrelevant columns 'adult', 'imdb_id', 'original_title', 'video' and 'homepage'.
handle stringified JSON column

#### 3.	Evaluate Python Expressions in the stringified columns ["belongs_to_collection", "genres", "production_countries", "production_companies", "spoken_languages"] and remove quotes ("") where possible.

### flatten nested Columns

#### 4.	Extract only the collection name from the column "belongs_to_collection" and overwrite "belongs_to_collection".
For example: The value in the first row (Toy Story) should be 'Toy Story Collection'.

#### 6.	Extract all spoken language names from the column "spoken_languages" and overwrite "spoken_languages". If a movie has more than one spoken language, seperate spoken languages by a pipe "|".
For example: The value in the first row (Toy Story) should be 'English'.

#### 7.	Extract all production countries names from the column "production_countries" and overwrite "production_countries". If a movie has more than one production country, seperate production countries by a pipe "|".For example: The value in the first row (Toy Story) should be 'United States of America'.

#### 8.	Extract all production companies names from the column "production_companies" and overwrite "production_companies". If a movie has more than one production company, seperate production companies by a pipe "|".For example: The value in the first row (Toy Story) should be 'Pixar Animation Studios'

#### 9.	Inspect all columns above with value_counts(). Do you see anything strange? Take reasonable measures!

### Cleaning Numerical Columns

#### 10.	Convert the datatype in the columns "budget", "id" and "popularity" to numeric. Set invalid values as NaN.

#### 11.	Analyze the columns "budget" and "revenue" and "runtime". Analyze movies with a budget/revenue/runtime of 0. Do you think the value 0 is the most appropriate value? Take reasonable measures!

#### 12.	The columns "budget" and "revenue" shall show values in Million USD. Convert and Overwrite!

#### 13.	Analyze movies with a vote_count of 0. What´s the vote_average for those movies? Do you think this value is the most appropriate value? Take reasonable measures!

### Cleaning DateTime Columns

#### 14.	Convert the datatype in the column "release_date" to datetime. Set invalid values as NaN.

### Cleaning Text / String Columns

#### 15.	Analyze the text columns "overview" and "tagline". Try to identify missing data that is not represented by NaN (e.g. "No Data"). Replace as NaN (np.nan)!

### Removing Duplicates

#### 16.	Identify and remove duplicates!

### Handling Missing Values & Removing Observations

#### 17.	Drop all rows/movies with unknown id or title.

#### 18.	Keep only those rows/movies in the df with 10 or more non-NaN values.

### Final (Cleaning) Steps

#### 19.	Keep only those rows/movies in the df with status "Released". Then drop the column "status".

#### 20.	The Order of the columns should be as follows:

#### 21.	Reset the Index and create a RangeIndex.

#### 22.	Save the cleaned dataset in a csv-file.

