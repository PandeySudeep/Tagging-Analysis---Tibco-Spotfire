# Tagging-Analysis-in-Tibco-Spotfire-via-Python
User Interaction can be customized via Python by tagging and untagging columns in data table.

Background
----------
Spotfire API allows selected rows in data table to be tagged with one or multiple tag names. This gives distinct identity to the rows. Visualizations or any actions can then take the tagged rows as input or create tagged rows as output operation. This been said - the concept can be utilized various ways by improvising. Once the data table is fully loaded, tagging/untagging can be done by marking, filtering, button click etc. In what different ways we could create user interaction and presentation is the matter of DESIGN.

Example
-------
The sample DXP attached herewith demonstrates a page 'Setup' which consists of a cross table analysis of financial data. On the left panel are multiple list box filters and down below the panel are two buttons 'Add selected account(s)' and 'Reset'. The first button triggers a python script (script1.txt) that takes the active filtering selection done by user, marks rows based on user selection and then tags columns and then resets the list box filter back programmatically. The second button 'Reset' triggers a python script (script2.txt) that brings the initial default state back by untagging all the rows.

Note
----

Point to note here is that data has already been pulled into spotfire dxp and user selection of multiple inputs in list box filter is effectless until first button is hit. This prevents any programmatic operation behind the scene during user selection and action is enabled only in the end of data selection via button click. Hence, optimized and interactive analysis can be achieved.
