# Finance Analyzer
Finance Analyzer is built to get maximum from your expenses. It provides comprehensive information about your charges. You can use detailed export to Excel and even database. Application has several built-in charts for tracking week and month activities. Distinctive feature of Finance Analyzer is an extended analytic: you can get detailed charts for every spending category. You can set custom start of the week and month, enable and disable coin support, export data in Excel and database file formats.

# Donate
If you would like to support the project feel free to donate. 
[Donate with PayPal](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=NHQJJCR7R6JEG).

# Credits
This ap is running awesome chart library for Android - [MPAndroidChart](https://github.com/PhilJay/MPAndroidChart/). Thanks to developers for such a great project.

# Usage
* [Main screen](#main-screen)
  * [Adding expense](#adding-expense)
  * [Removing expense](#removing-expense)
* [Statistics and charts](#statistics-and-charts)
  * [Monthly top](#monthly-top)
  * [Weekly top](#weekly-top)
  * [All-time top](#all-time-top)
  * [Numbers only](#numbers-only)
* [Import and export](#import-and-export)
* [Settings and configuration](#settings-and-configuration)

## Main screen
On the main screen there are the list of recorded expenses. It is scrollable so you can see the history with latest added items at the top. 
At the top of the screens there are navigation pane with icons for statistics, import & export, settings. There are also HIDE DATA switch. Press it if you want to hide expense list. 
At the bottom of the screen there are EXPENSE button. Press it to record new expense. 
![Main screen](http://i.imgur.com/tPO0YVg.png)

## Adding expense
The steps for adding new expense are easy:
1. Set expense name in the first text box
2. Set the price in amount text box
3. Set label. Label indicates the spending's category. 
![Adding expense](http://i.imgur.com/ESdl304.png)
Every text box has automcomplete. It goes through all of the previous spending and looks for names match. If you already have the expense with same name, the application will set the amount and label automatically based on the previous expense data. However, you can override the amount and label manually.
![AutoComplete](http://i.imgur.com/OS4crNw.png)

## Removing expense
In order to remove the expense go to the main screen and find the expense in the list. Perform long press (long click) and select OK in pop-up Delete Expense dialog.
![Removing expense](http://i.imgur.com/xxc5Pf9.png)
![Removed](http://i.imgur.com/bhkiIbx.png)

## Statistics and charts
To start exploring statistics select chart type first.
![Chart selector](http://i.imgur.com/pn63RyZ.png)

### Monthly top
Pie chart for all labels from the start of the current month (see Settings and configuration for details). 
![Monthly top](http://i.imgur.com/KynvQIv.png)
Click on label sector to see the expenses.
![Label details](http://i.imgur.com/vEtzb4C.png)
Expenses from selected label. Click on expense to see detailed report on it in bar chart. X axis is amount, Y axis is day of month.
![Expense details](http://i.imgur.com/wJgPlF3.png)

### Weekly top
The same as monthly top but from the start of the week (see Settings and configuration for details).

### All-time top
The same as monthly and weekly top but from the very start of application usage. Pie chart with all expenses.

### Numbers only
Keeps the following data:
* Expenses count in database
* Total amount of money spent
* Average expense amount
* Median expense amount (in development)
* Maximum amount recorded for one expense
* Minimum amount recorded for one expense

## Import and export
At the moment, only export supported in Microsoft Excel (.xls) and SQLite database file (.db). For exporting data please select the file type and press Export button. Default export location: sdcard/Finance Analyzer/
![Export](http://i.imgur.com/WM8g0PY.png)
After the export is finished the message with file location should appear.
![Exported](http://i.imgur.com/gtwaEdF.png)

## Settings and configuration
The following settings supported: 
* First day of week. Used for weekly top labels chart. Default: Monday
* First day of month. Used for monthly top labels chart. Default: 1
* Coin support. Changes amount format to display coins (cents). Default: false
![Settings](http://i.imgur.com/ldOIfIV.png)
