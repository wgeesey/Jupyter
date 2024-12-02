# Jupyter



### Interactive Visualizations with Ipywidgets
This repository contains a series of interactive visualizations using ipywidgets in Python (or notebooks) that I have worked on during my Data Science and Jupyter journey.

#### The examples demonstrate how to create interactive elements within Jupyter Notebooks:

Sine Wave Visualization: Interactive plots of sine waves with adjustable frequency sliders.
Language Selector: A dropdown menu to select and display programming language descriptors.
Value Display: A simple interactive widget to return and display a value.
Integer Slider: An integer slider for dynamic value selection.
Button Clicks: Interactive buttons to select and display a favorite programming language, with clear output functionality.
Styled Buttons: Enhanced button UI with custom styles and layout


## soccer.ipynb

### FIFA 23 Data Analysis
#### Overview
In this project, I worked with the FIFA 23 dataset from Kaggle, which includes player statistics like ratings, value, and wages. The goal was to clean the data and explore the relationship between a player's wages and their value, helping to uncover interesting patterns and insights.

#### What I Did
Data Preprocessing:

Selecting Relevant Columns: First, I created a new dataset that focuses only on the columns that matter for this analysis: Name, Overall, Potential, Wage, and Value.
Cleaning the Wage and Value Columns:
Both of these columns had some unwanted characters, like the Euro sign (€) and commas. I removed them so I could work with just the numbers.
The Wage and Value columns also had abbreviations like 'K', 'M', and 'B' to represent thousands, millions, and billions. I used a function to convert these into actual numbers so they could be analyzed properly.
Handling Missing or Messed Up Data: In cases where the data couldn’t be cleaned or converted correctly (like weird characters or missing values), I replaced it with 0.0 to avoid errors.
Creating New Columns:

Difference Column: I added a new column that shows the difference between a player's Value and Wage. This is useful to see if some players are getting paid more than they’re worth (or vice versa).
Data Filtering:

Top Players by Rating: I filtered out the top players with an Overall rating above 90. This helped me focus on the best-performing players in the dataset and see how their wages compare to their value.
Sorting and Displaying the Data:

I sorted the data based on the new Difference column so I could easily identify players who are overpaid or underpaid compared to their value.

#### What I Found
After cleaning the data, I was able to see how players’ wages compare to their value, and it was interesting to identify players who might be getting overpaid or underpaid. A negative 'Difference' means the player is getting paid more than their 'Value', a positive means they 
are valued higher than their wage.
By filtering for players with an Overall rating above 90, I could focus on the best players and see how their wages line up with their market value (was just a test to see how it would work).
##### Dependencies
pandas: For handling and manipulating the data.
numpy: For working with numerical data.
