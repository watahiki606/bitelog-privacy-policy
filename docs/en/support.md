# BiteLog Support Page

## App Overview

BiteLog is an application that allows you to easily track your daily calorie and macronutrient (protein, fat, carbohydrates) intake through daily meal logging.
By utilizing the search function for past meal data and the CSV import function, you can more easily manage your daily diet.

## Main Features

### Meal Logging

- **Simple Input Form:** You can manually enter brand name, product name, amount, unit, and nutritional information.
- **Search Past Meals:** You can search and reuse past meal data that you have registered.
- **Meal Type Classification:** You can record meals by classifying them into four meal types: Breakfast, Lunch, Dinner, and Snack.
- **Daily View:** You can select a date in a calendar format and view a list of meal records for that day.
- **Automatic Nutrient Calculation:** Based on the nutritional information of the registered food, the app automatically calculates the total values of calories, protein, fat, and carbohydrates, and displays them daily and by meal type.

### CSV Import

- **Batch Registration of Data from CSV Files:** You can batch import past meal data from CSV format files into FoodMaster (food master data) and LogItem (meal record data).
- **Supported CSV Format:**
    ```
    date,meal_type,brand_name,product_name,calories,carbs,fat,protein,portion_amount,portion_unit
    2024-03-20,Breakfast,Brand A,Product B,200,30,10,8,1.0,piece
    ```
    - **date:** Date (YYYY-MM-DD format)
    - **meal_type:** Meal Type (Breakfast, Lunch, Dinner, Snack)
    - **brand_name:** Brand Name
    - **product_name:** Product Name
    - **calories:** Calories
    - **carbs:** Carbohydrates
    - **fat:** Fat
    - **protein:** Protein
    - **portion_amount:** Portion Amount (numeric)
    - **portion_unit:** Unit (piece, g, ml, etc.)
- **Import Procedure:**
    1. Select "CSV Import" from the app's settings screen.
    2. Check the explanation of the CSV file format and tap the "Select CSV File" button.
    3. Select the CSV file you want to import from the file picker.
    4. Import will start, and the results will be displayed upon completion.

### Language Settings

- **Multilingual Support:** Supports Japanese and English.
- **System Settings Integration:** By default, the app is displayed in the language according to system settings.
- **In-App Language Switching:** You can switch the display language of the app from the settings screen.
    - If you change the language setting, you will need to restart the app.

### Data Management

- **Data Deletion:** You can delete all recorded data from the settings screen.
    - Please note that data deletion cannot be undone.

## FAQ

**Q: CSV import is not working.**

A: Please check if the CSV file format is correct.
Referring to the "Supported CSV Format" section above, please check if the CSV file is described in the specified format.
In particular, check whether the header line (`date,meal_type,brand_name,product_name,calories,carbs,fat,protein,portion_amount,portion_unit`) is included, whether the delimiter for each item is a comma ',', and whether the date format is YYYY-MM-DD format.

**Q: No results are displayed when searching past meals.**

A: Please check if your search keyword is correct and if meals have been registered in the past.
You can search by brand name or product name.
Also, if you have never registered a meal in the past, no search results will be displayed.

**Q: Can I add my own units other than "g" or "piece"?**

A: Yes, you can freely add units.

## Contact Us

If you have any questions or problems, please contact us via the inquiry form in the app settings screen or at the email address below.

[Email Address] (e.g., support@bitelog.example.com)

## Future Update Plans

- Free addition of units function
- Enhanced reporting features (weekly nutrient intake reports, etc.)
- iCloud synchronization function

Thank you for your continued support of BiteLog.
