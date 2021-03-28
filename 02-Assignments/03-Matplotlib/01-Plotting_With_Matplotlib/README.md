
# 3.1 Skill Drill: Pymaceutical Data Analysis 

In this week's Skill Drills, you will act the part of a data analyst at Pymaceuticals Inc., one of the leading imaginary pharmaceutical companies that specializes in anti-cancer pharmaceuticals. You have been hired to assist their senior scientist team in the effort to begin screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

In this study, 249 mice that identified with SCC tumor growth were treated through a variety of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals' drug of interest, Capomulin, versus other treatment regimens. You have been tasked by the senior scientist team to generate an initial drug regimens comparison and generate a summary of your findings. 

For this skill drill, you will perform basic analysis and visualize the dataset using a new type of visualization - a box and whisker plot. Although you have been provided all of the steps required to produce each output, there may be some new or unfamiliar concepts and terminology in this skill drill. If you are ever stuck or confused, try researching some of the terms or check out the resource links provide throughout the activity. You got this!

### Instructions:

**Part 1:** Data Cleaning
     
1. Load the dataset into the notebook.

    * There are two datasets located in the Resources folder:
      * Mouse_metadata.csv
      * Study_results.csv
    
    * Display both datasets once you loaded each into Pandas. 

2. Merge the data together into one DataFrame.

    * Combine both data frames into one and display it.

3. Clean the the data for any mouse ID with duplicate time points and remove any data associated with that mouse ID.

      * **Hint:** Use Pandas DataFrame `.duplicated()` method to identify which rows have duplicated `Mouse ID` and `Timepoint` columns. Find the `Mouse ID` associated with these duplicate rows.

      * **Optional**: Display the data generated by the duplicated `Mouse ID`.

      * Create a clean DataFrame by dropping any rows that contain the duplicated `Mouse ID`.

**Part 2:** Data Analysis and Visualization

4. Isolate the final timepoint for each mouse.

    * **Hint:** Try using a Pandas `GroupBy` DataFrame and the `.max()` method to determine the largest `Timepoint` for each `Mouse ID`.
    
    * Reset the index of the Pandas DataFrame. 

       * **Hint:** Look at the Pandas documentation for [resetting an index](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.reset_index.html).
    
    * Join the newly created `.max()` DataFrame (the one you just assigned to a variable) with the DataFrame from Part 1 (the one in which you dropped the duplicated mice) to get the tumor volume at the last timepoint.
      
5. Calculate the final tumor volume of all mice in the study across all drug regimens.

    * Create a list with all 10 drug regimens.

    * Create an empty list to fill with tumor volume data.
    
    * Create a for loop to iterate through the drug regimen list.

    * Isolate (filter) each mouse on each drug to collect their tumor volume. 

      * **Hint:**: Use Pandas `.loc` method to filter your DataFrame by checking which of the current drugs is equal to the `Drug Regimen` column. See [these examples on how to select and filter data using `.loc`](https://www.allthesnippets.com/browse/pandas/df_selection.html).

    * Append the outcome to the empty list previously created.
        
6. Create a boxplot that visualizes the final tumor volume of all mice in the study across all drug regimens.

    * Create a horizontal Matplotlib box and whisker plot using the `plt.boxplot()` method. 

      * **Note:** To make your boxplot horizontal, use the `vert=False` argument. See the Matplotlib [boxplot documentation](https://matplotlib.org/api/_as_gen/matplotlib.pyplot.boxplot.html#matplotlib.pyplot.boxplot) for more information. 

    * Show your plot in the notebook.

* **Part 3:** Critical Thinking 

7. Now that you have created your first box and whisker plot, it's time to interpret your results. Take a look at the article linked below about the different components of a box and whisker plot. Compare these components to that of your own plot and consider the following questions. For now, there is no need to write out and submit any answers for these questions. 

  * [Towards Data Science: Understanding Box Plots](https://towardsdatascience.com/understanding-boxplots-5e2df7bcbd51)

    * What do the distribution of final tumor volumes look like for each regimen. Are there one or two drug regimens that look different from the other regimen results? 
    
    * What does it mean when a box of one drug regimen is smaller than another? Does that mean that data is missing? Why or why not?

    * **Note:** Do not worry if you do not recognize all of the different statistical measurements, we will cover them in the next unit! 

---

© 2021 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.