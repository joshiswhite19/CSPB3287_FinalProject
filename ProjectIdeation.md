# CSPB-3287 Final Project
## Initial Project Ideation
## Josh White
## 2/14/2022
My initial idea for my final project is to develop a Hot Sauce Recipe Book and supply management database, which I could eventually use to actually help me track and manage all the hot sauces I have developed and want to continue making.

### This database will tentatively have four different tables, with the following attributes:

1. Hot Sauce Recipe Table: Recipes
- Sauce ID (Primary Key)
- Name
- Description
- Preparation Time
- Ingredient 1 Name
- Ingredient 1 Quantity
- etc....

2. Current Supplies List: Supplies
- Item Name (Primary Key)
- Quantity
- Quantity Units
- Expiration Date

3. List of Sauces planned to Prepare: PlannedPrep
- Preparation entry ID (Primary Key)
- Sauce ID to prepare
- Prep Start Date
- Number of sauce batches planned

4. List of Supplies to Purchase: RequiredPurchase
- Purchase entry ID (Primary Key)
- Supply Name
- Quantity to Purchase
- Need date

### The following steps describe basically how the database would work:

1. Enter a new sauce recipe into Recipes
2. Add supplies to the Supplies list
3. Add a sauce already in the Recipes list to the PlannedPrep list
4. Some checking will be performed based on the planned sauce recipe and what is currently in the supplies list and an entry will be added to the RequiredPurchase list for anything required to make the planned sauce
5. When supplies are updated in the Supplies list, the RequiredPurchase list is checked to see if an entry is addressed and delete any entries that were addressed

### Database and other planned tools:

My tentative plan will be to create a local MySQL database (so nobody can steal my highly advanced sauce recipes), but my project will include all the table definitions for starting a new database on the computer of whoever uses the project. I will do all of my development in a Jupyter notebook so that I can include notes for usage of the database and also include any additional tools I may need to implement in Python.

### What I hope to learn from this project:
From this project I hope to learn how relational databases can be used to manage the logistics of a small operation that includes the storage and consumption of supplies, and tricks for how those lists can be updated and maintained in a smart way. Although making a list to track my hot sauce recipes is personally interesting to me, this type of database can easily be extended to other situations.
