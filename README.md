# To-Go-Simulating-a-Fast-Food-Environment
### *Introduction*
I am excited to share my latest project, To-Go, a Python-based fast-food simulation program. In this project, I have designed a program that creates a virtual fast-food environment, allowing users to interact with a menu, add products, make purchases, and more. This project aims to provide an immersive experience, replicating the functionalities of a fast-food restaurant in a simulated setting. Let's dive into the details of this exciting venture!

### **Section 1**

**Data Loading and Manipulation** 

To begin, I loaded two data files in CSV format from a Dropbox repository. The first file, "menu.csv," contains the menu item codes and the available quantities of each product. The second file, "foods.csv," includes information about food names, categories, and prices. I standardized the column names in both datasets to ensure consistency and merged them into a single data frame for further processing.

**Standardizing the Column Names:** I addressed inconsistencies in the food names by creating a function that cleaned the food entries in the "foods" data frame. The function removed the brand name and capitalized the food names to match the format in the "menu" data frame. This standardization process ensures uniformity in the data.

**Merging the Datasets:** Next, I merged the standardized data frames using an outer join, with the "menu_number" column serving as the index for the new table. This merged data frame combines information from both files, enabling efficient access to all relevant data in a single structure.

**Changing Values in a Data Frame:** To accommodate a small oversight, I added three units of "Chips" to slot B4 in the merged data frame. This adjustment ensures that the inventory accurately reflects the availability of products.

### **Section 2**

Fast-Food Simulation Program: With the merged data set as the foundation, I implemented a fast-food simulation program that offers several options for users to interact with the virtual environment.
1.	Admin Login: This option simulates the validation of admin credentials. Users are prompted to enter a username and password, with the username set as "admin" and the password as any number less than 10. The program allows four login attempts, and upon successful login, the option becomes disabled.
2.	Add Products: After logging in as an admin, users can select this option to add one more product to a specific menu slot. The program displays the current food menu and prompts the admin to input a menu number. The program handles various scenarios, such as full slots, empty slots, and the maximum limit of eight products per slot. After adding a product, the updated food menu is displayed.
3.	Buy Food: This option allows any user to purchase food items from the virtual menu. The program displays the available food items, their quantities, and prices. Users can select a food item by entering its menu number. The program validates the selection and calculates the payment amount. Users enter the payment and receive change if applicable. The program updates the inventory based on the purchase and provides feedback on the number of products left.
4.	Exit: Users can choose this option to exit the fast-food simulation program.

### **Conclusion**
To-Go provides an engaging and interactive fast-food simulation experience. By implementing various functionalities, such as admin login, product addition, and food purchase, the program replicates the operations of a real fast-food environment. The project showcases the power of Python and demonstrates how data manipulation and program design can create immersive simulations. I thoroughly enjoyed working on this project, and I hope you find it interesting and insightful. Stay tuned for more exciting projects and updates! Feel free to reach out if you have any questions or suggestions.
