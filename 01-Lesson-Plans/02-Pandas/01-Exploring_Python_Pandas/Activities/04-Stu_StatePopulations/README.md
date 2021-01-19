# State Populations

In this activity, you will manipulate Pandas DataFrames. This skill is useful when, for example, you need to view the first few lines of a dataset without opening the whole dataset. 

## Instructions:


1. Start by importing your dependencies.

    * `import pandas as pd` and `import os`

2. After importing your dependencies, open the [state_list_with_population.csv](Activities/04-Stu_StatePopulations/Resources/state_list_with_population.csv) and create a new DataFrame with the data.

3. Use the `.head()` function to display the data in the following ways:

    * Return the head of the DataFrame with all columns.

    * Return the head of a single column in the DataFrame.

    * Return the head of the `state_abbreviation` and `population` columns in the DataFrame.

    * Slice the DataFrame using the `.loc[]` function on the `state_abbreviation` and `population` columns.

    * Slice the DataFrame using the `.iloc[]` function on the `state_abbreviation` and `population` indexes. 

4. **Bonus**: Print out the states that have a population greater than 5,000,000 using `.loc[]`

---

© 2021 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
