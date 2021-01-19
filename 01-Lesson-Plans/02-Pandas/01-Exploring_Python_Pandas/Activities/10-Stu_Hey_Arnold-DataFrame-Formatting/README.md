# Hey, Arnold!

You won't always have data in a perfect state. Sometimes, you will need to manipulate and slice it  to get it into the state you need for your project. In this activity, you will take a pre-made DataFrame of characters from the animated television series ["Hey Arnold!"](https://en.wikipedia.org/wiki/Hey_Arnold!) and reorganize it so that it is more comprehendible and organized.

## Instructions

1. Start by using Pandas to create a DataFrame with the following columns and values:

    * `Character_in_show`: Arnold, Gerald, Helga, Phoebe, Harold, Eugene

    * `color_of_hair`: blonde, black, blonde, black, unknown, red

    * `Height`: average, tallish, tallish, short, tall, short

    * `Football_Shaped_Head`: True, False, False, False, False, False

2. The above column names are inconsistent and difficult to work with. Rename them to the following, respectively:

    * `Character`, `Hair Color`, `Height`, `Football Head`

3. Create a new table that contains all the columns in the following order:

    * `Character`, `Football Head`, `Hair Color`, `Height`

4. **Bonus**: Use the lambda `apply()` function to highlight if the row contains a football-shaped head. 

    * Here is a resource for how to highlight a row in Pandas: [Pandas Style Guide](https://pandas.pydata.org/pandas-docs/stable/user_guide/style.html)


---

© 2021 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
