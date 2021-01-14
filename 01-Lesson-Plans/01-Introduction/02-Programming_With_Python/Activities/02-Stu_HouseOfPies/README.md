# House Of Pies

In order to build Python scripts capable of performing complex data workflows, we need to know how to combine loops, conditionals, and try-except blocks. For this activity, you will leverage your Python programming knowledge in order to create an inventory management system for our new start-up bakery business. 

## Instructions

1. Create a dictionary that stores a value of `10` for each of the following pie names: 

    * `Pecan`, `Apple`, `Blueberry`, `Pumpkin`, `Chocolate`

    * **Note:** This dictionary will act as your "inventory of pies". 

2. Create a series of print statements that will welcome and display a list of pies to the user in the following way:

    ```
    Welcome to the House of Pies! Here are our pies:
    ---------------------------------------------------------------------
    (1) Pecan, (2) Apple, (3) Blueberry, (4) Pumpkin, (5) Chocolate
    ```

3. Create a while-loop that performs the following logic:

    * First prompt the user to make a numerical selection using `input()` and store the user's selection to a variable. 

      * **Hint:** If you have never used the `input()` function before, check out some helpful documentation [here](https://www.w3schools.com/python/ref_func_input.asp).

      * A good input statement should include some text explaining the user prompt such as, `Please make a selection:`

    * Create a series of `if-else` statements that convert the numerical selection to the correct name of the pie. 

      * **Hint**: When using a series of `if` and `else` statements, try using `elif` which combines `else if` into one step. You can read more about `elif` statements here: [here](https://www.w3resource.com/python/python-if-else-statements.php). 

    * Simulate an order by removing a pie from your inventory that matches a user selection. 
      
      * In the context of this activity, a pie is sold out when it's inventory equals zero.

      * If you try to remove a pie that is sold out, you need to raise an exception and print the following statement back to the user: `Sorry that pie is sold out.`

      * If the pie is not sold out, remove one pie from your inventory and print the following statement back to the user: `Order received.`

## Bonus (Optional)

4. When you raise an exception in your `while` loop, print out the names of any non-zero pies remaining in the inventory as a suggestion to the user. 

5. Update your `while` loop logic to stop running when all inventory equals zero.

---

© 2021 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
