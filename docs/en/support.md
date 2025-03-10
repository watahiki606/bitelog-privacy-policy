## App Overview

BiteLog is a simple meal tracking app. By recording meals, it visualizes eating habits and promotes awareness towards a healthier diet.

## Main Features

### Meal Recording

- **Simple Input Form:** Manually enter brand name, product name, amount, unit, and nutritional content.
- **Search from Past Meals:** Search and reuse previously logged meal data.
- **Meal Type Classification:** Meals can be categorized into four types: breakfast, lunch, dinner, and snacks.
- **Daily Display:** Select dates using a calendar format to view meal records for that day.
- **Automatic Nutrient Calculation:** Automatically calculates total calories, protein, fats, and carbohydrates based on the nutritional content of registered foods, displayed daily and by meal type.

### CSV Import

- **Bulk Data Registration from CSV Files:** Import past meal data into FoodMaster (food master data) and LogItem (meal record data) from a CSV file.
- **Supported CSV Format:**
    ```
    date,meal_type,brand_name,product_name,calories,carbs,dietary_fiber,fat,protein,portion_amount,portion_unit
    2024-03-20,Breakfast,Brand A,Product B,200,30,5,10,8,1.0,each
    ```
    - **date:** Date (YYYY-MM-DD format)
    - **meal_type:** Meal type (Breakfast, Lunch, Dinner, Snack)
    - **brand_name:** Brand name
    - **product_name:** Product name
    - **calories:** Calories
    - **carbs:** Total carbohydrates
    - **sugar:** Sugars (part of carbohydrates)
    - **dietary_fiber:** Dietary fiber (part of carbohydrates)
    - **fat:** Fats
    - **protein:** Protein
    - **portion_amount:** Portion size (numeric)
    - **portion_unit:** Unit (each, g, ml, etc.)
- **Import Procedure:**
    1. Select "CSV Import" from the app's settings menu.
    2. Review the format of the CSV file and tap the "Select CSV File" button.
    3. Choose the desired CSV file from the file picker.
    4. Import begins, and results are displayed upon completion.

### Language Settings

- **Multilingual Support:** Supports both Japanese and English.
- **Integration with System Settings:** By default, the app displays in the language set in the system settings.
- **In-app Language Switching:** You can switch the display language of the app from the settings menu.
    - Changing the language setting requires restarting the app.

### Data Management

- **Data Deletion:** All record data can be deleted from the settings menu.
    - Please note that data deletion is irreversible.

## Nutrient Calculation Method

In BiteLog, carbohydrates are calculated as the sum of "sugars" and "dietary fiber." When both carbs and dietary fiber are specified during CSV import, sugars are automatically calculated as "carbs - dietary fiber."

## FAQ

**Q: The CSV import is not working.**

A: Please check if the CSV file format is correct. Refer to the "Supported CSV Format" section above and ensure that the CSV file is written in the specified format. Specifically, check if the header line (`date,meal_type,brand_name,product_name,calories,carbs,dietary_fiber,fat,protein,portion_amount,portion_unit`) is included, if the items are separated by commas `,`, and if the date is in the YYYY-MM-DD format.

**Q: No results are displayed when I search for past meals.**

A: Check if the search keyword is correct and if meals have been registered in the past. You can search by brand name or product name. If no meals have been registered before, no search results will be displayed.

**Q: Can I add units other than 'g' or 'each'?**

A: Yes, users can freely enter units. When registering food, you can input any unit (e.g., "pack," "slice," "cup") in addition to common units like 'g' or 'each'.
