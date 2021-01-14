# Solving Data Problems With Python

When it comes to building powerful scripts and programs in Python, there is power in numbers! We need to rely on the many internal and external libraries, modules and documentation in order to succeed. In this activity, you will read a tab-delimited file containing 1000 Netflix titles, manipulate values within the rows and then export the manipulated table into a comma-delimited CSV file.

## Instructions

1. First, import the `os` and `csv` libraries into your notebook.

2. Use `os.path.join` to build both the path to your tab-delimited `netflix_ratings.txt` file, and an outfile named `netflix_ratings_cleaned.csv` in the `Resources` folder of this activity.

3. Once you have created your paths, open a connection to the tab-delimited import file and the comma-delimited export file using the `open()` function.

4. Create your instances of `csv.reader()` and `csv.writer()` methods to import and export your files.

   * **Hint:** The table file we are importing is not comma-delimited. Rather, it is `\t` tab-delimited. How would you modify your `csv.reader()` method to accommodate this difference? 

5. Read in your column header row and remove the `ratingLevel` column from your list of column headers.

6. Write out your new header row to the new comma-delimited outfile.

7. Iterate through each row of your import file and apply the following changes. Once you apply these changes to each row, print the row in your Python notebook and write the row out to the new comma-delimited outfile.


   * Concatenate the second and third columns in each row using a hyphen `-` to make a single `rating` column. Set this concatenated string to the second column in each row.

   * Remove the third column from each row.

   * Check if the fifth column in each row is equal to `"NA"`. If so, replace the fifth column value with a value of `"50"`.

## Bonus (Optional)

8. If you are familiar with importing and exporting using `csv`, or if you want an additional challenge, try exporting your table into a **JavaScript Object Notation** (**JSON**) format using the `csv` library along with the built-in `json` library. A few notes on using the `json` library:

   * If you export to a `json`, change your filename to `netflix_ratings_cleaned.json`. 

   * Instead of using the `csv.reader()` to handle each row in our import file, use the `csv.DictReader()` class. This class will convert each row into an ordered Python dictionary. A Python dictionary is very similar to the structure of a JSON object and is required when using the `json` library to export. 

   * The `json` library does not write each row to the output file individually like `csv.writer()`. Instead, you will write the entire file out at once using the `.write(json.dumps())` method from your connected output file. Therefore, you will need to create an empty dictionary at the top of your Python notebook and fill it with each row.
  
   * Because each row is converted to a dictionary, you must concatenate the `rating` and `ratingLevel` column, set `row["rating"]` to this concatenated value, and drop the `ratingLevel` using the `row.pop("ratingLevel")` method. 

   * Similarly, your rows are using the header names as the key for your row dictionary. Therefore, in order to check whether or not the fifth column is equal to `"NA"`, you must use the `user rating score` instead of the relative index.

   * To see a great example of exporting a CSV file to a JSON file using the `json` library, check out this article: [Programiz: Python JSON](https://www.programiz.com/python-programming/json). 


---

© 2021 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
