# tenis-tournaments
Script for generating Unique Doubles For Tournaments

## How to Use This Script

Open your Google Sheet with the player data
Click on "Extensions" in the menu and select "Apps Script"
Replace any existing code with this script (or add this as a new function if you want to keep the singles script too)
Save the project
Return to your spreadsheet and refresh the page
You'll see a menu item called "Pari" with two options now: one for singles and one for doubles


### Important Notes:

Your player names should be in column A (starting from row 2)
You must have a number of players divisible by 4 for doubles
The script creates a new sheet called "Dvojice" with the generated pairings
The algorithm ensures:

No player pairs with the same partner twice
No player faces the same opponent twice
The script considers A-B vs C-D to be the same as B-A vs D-C (order doesn't matter)

The script includes a limit to prevent infinite loops in case a perfect solution isn't possible. If it can't find a complete set of pairings, it will show how many rounds were successfully generated.
