## Step 1: Project GitHub Copilot agent mode

Welcome to your **"California AI Policy Analysis"** Repository! :robot:

### Project Libraries List

In this step we will create a list of project libraries for R

```prompt
We will create a list of R libraries required by the project. The required libraries are:
"lubridate", "jsonlite", "dplyr", "magrittr", "R6", "haven", "labelr", "plyr", "stringr", "purrr", "glue", "Hmisc", "psych", "tibble", "here", "tidyr", "knitr", "labelled", "collapse", "formattable"
We want to create a json file containing these libraries for the project, and store the list on the 'metadata' directory of the project. The JSON file should be named 'libraries.json'. The library list should be put into the root of the JSON file (no parent).
```

### AI Bills Lists

Here, we will create a set of lists for AI bills in the California Legislature.

```prompt
Using the list of bills by legislative session below, we need to create a JSON file containing the legislative session, and each of the bills below. The JSON file should be stored in the 'metadata' directory of the project, and named 'aiBillList.json'
- Y20132014: "SB-836", "SB-860", "AB-1465"
- Y20172018: "ACR-215", "SB-1470", "AB-2662", "AB-1809", "SB-843"
- Y20192020: "SB-348", "SJR-6", "AB-459", "AB-1576", "AB-976", "AB-594", "SB-444", "SB-730", "AB-156", "AB-3317", "SCR-13", "ACR-125", "SB-752", "AB-2269", "AB-3339", "AB-485"
- Y20212022: "SB-1216", "AB-2224", "AB-587", "SR-11", "AB-2826", "AB-1545", "AB-1400", "SB-54", "AB-1651", "AB-1// #region prompt
- Y20232024: "AB-2652", "SB-1288", "AB-2013", "AB-2811", "SB-893", "SB-1235", "SB-896", "SB-313", "SB-970", "AB-3030", "SB-1229", "SB-1120", "SB-398", "AB-3058", "SB-1047", "AB-3204", "AB-2876", "AB-2885", "AB-3095", "AB-1831", "SB-942", "ACR-96", "SB-933", "SB-892", "AB-2355", "SB-1381", "AJR-6", "AB-1873", "SCR-17", "AB-2905", "AB-3050", "AB-3211", "AB-2877", "AB-331", "SB-1220", "AB-2512", "ACR-227", "AB-2930", "AB-1027", "AB-302", "SCR-121", "AB-2412", "AB-2839", "ACR-219", "SB-1446", "SCR-162", "SB-1154", "AB-2655", "AB-1008", "AB-1526", "AB-2200", "SB-1223", "AB-108", "AB-103", "AB-2928", "AB-100", "SB-100", "SB-103", "AB-106", "SB-158", "SB-106", "AB-158", "AB-104", "SB-104", "SB-107", "AB-107", "AB-1754"
- Y20252026: "SB-813", "SB-833", "SB-579", "AB-316", "SB-524", "SB-366", "SB-420", "SB-11", "SB-468", "AB-412", "AB-1064", "AB-489", "AB-512", "AB-979", "AB-853", "AB-1405", "AB-410", "SB-243", "SB-503", "SB-53", "AB-222", "SB-238", "AB-1159", "AB-1137", "AB-682", "SB-711", "AB-93", "SB-7", "AB-723", "AB-1024", "AB-279", "AB-1018", "AB-1242", "AB-392", "SJR-2", "AB-325", "SB-57", "SB-295", "AB-887", "AB-1170", "SB-354"
```

:recycle: If needed, update the list of bills above and re-run the prompt on GitHub Copilot Agent.

### LC Bills Lists

```prompt
Using the list of bills by legislative session below, we need to create a JSON file containing the legislative session, and each of the bills below. Before storing the bills, we want to make sure there are no duplicate bills, and we need to re-order the bills in the JSON file, by their name. The JSON file should be stored in the 'metadata' directory of the project, and named 'lcBillList.json'. 
The list of bills should be put into the root of the JSON file (no parent key).
Here's the list of bills:
"AB-21", "AB-33", "AB-96", "AB-231", "AB-283", "AB-288", "AB-303", "AB-331", "AB-339", "AB-340", "AB-346", "AB-423", "AB-424", "AB-427", "AB-478", "AB-495", "AB-522", "AB-569", "AB-571", "AB-596", "AB-672", "AB-711", "AB-853", "AB-882", "AB-1054", "AB-1067", "AB-1109", "AB-1189", "AB-1323", "AB-1331", "AB-1355", "AB-1383", "ACA-1", "ACA-2", "SB-7", "SB-16", "SB-21", "SB-23", "SB-27", "SB-28", "SB-35", "SB-36", "SB-37", "SB-70", "SB-82", "SB-83", "SB-237", "SB-238", "SB-299", "SB-301", "SB-309", "SB-366", "SB-458", "SB-481", "SB-600", "SB-853", "SJR-2"
```

:recycle: If needed, update the list of bills above and re-run the prompt on GitHub Copilot Agent.

### Step 2: Run preliminary R functions

In this step, we will create a set of preliminary R functions to be used in the project.

```prompt
We will be using the script "ProjectFunctions.R" located in the `scripts/bills` directory.
1. Open the R interactive terminal.
2. Source the script "ProjectFunctions.R" using the `source()` function.
3. Verify that the functions defined in the script are loaded into the R environment.
4. Test the functions to ensure they work as expected for the project.
```

### Add Template for AI Bills
