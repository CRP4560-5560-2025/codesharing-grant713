CODE-SHARING ASSIGNMENT TOOLBOX

Author: Grant Rednour
Date Created: 12/2/2025

Purpose:

This toolbox allows a user to:
	Select a CSV file and a GeoJSON file.
	Convert the GeoJSON into a feature class.
	Join the CSV to the feature class and preserve all CSV rows.
	Create a graph from numeric fields in the joined data.
	It is designed to run in ArcGIS Pro using a Python toolbox (.pyt).

Toolbox Steps
	Step 1 — Select Input Files
	Choose your CSV file - Population_State_Story_County_CRP4560.csv
	Choose your GeoJSON file - P504577759-2025-11-2009564883-MapLayer
	Specify an output folder for generated files (EX.  Output)
	Click Run to complete Step 1.

Note: Step 2 depends on the outputs selected here.
Step 2 — Convert GeoJSON to Feature Class
	Select the GeoJSON file (from Step 1  - P504577759-2025-11-2009564883-MapLayer)
	Select the output folder (from Step 1) - (Output)
	Click Run to convert the GeoJSON into a feature class.
	A new feature class called Converted_GeoJSON will be created in the output folder.

Step 3 — Join CSV to Feature Class
	Select the feature class created in Step 2 - Converted_GeoJSON
	Select the CSV file (from Step 1) - Population_Stats_Story_County_CRP4560
	Choose the join field in the feature class - NAME
	Choose the join field in the CSV - Geometry (case sensitive)
	Specify an output CSV file path - select an output folder
	Select a display option: Show All
	Click Run to create a CSV with the joined data.
	Notes:
		All rows from the CSV are preserved (left join).
		Make sure the join fields exist in both the CSV and feature class.

Step 4 — Create Graph
	Select the CSV or feature class to graph (output from Step 3)
	Select the X field NAME.
	Select the Y field MEDIAN AGE.
	Specify the output folder to save the graph PNG.
	Click Run to generate the graph.
	Notes:
		Only numeric fields are available for selection.
		The graph is saved as graph.png in the selected folder.


Always run steps in order (1 → 4)
