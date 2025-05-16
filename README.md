# Tableau-VGS-

Table of Contents<br>
Introduction<br>
Dashboard Requirements<br>
Installation / Usage<br>
DAX Formulas Used in Measures<br>
Bug / Feature Request<br>
Authors<br>

<b>Introduction</b><br>
This dashboard provides an interactive analysis of video game sales across genres, platforms, publishers, and years. It helps users explore:<br>
Total sales by genre, platform, and game title.<br>
Yearly sales trends.<br>
Top-selling publishers and platforms.<br>
Filtered insights by region, time, and genre.<br>
It is built using Tableau to visualize historical sales data and identify business patterns in the gaming industry.<br>

<b>Dashboard Requirements</b><br>
To view and interact with this dashboard, you’ll need:<br>
Software: Tableau Desktop (version 2021.1 or higher recommended).<br>
File: Video game sales.twbx.<br>
Dataset: vgsales.csv (or included dataset in .twbx if packaged).<br>
System Requirements: 4GB+ RAM, Windows/macOS, Tableau-compatible system.<br>

<b>Installation / Usage</b><br>
Open Tableau Desktop.<br>
Open the file Video game sales.twbx.<br>
Ensure the data source is connected (or replace it with your copy of the CSV if necessary).<br>
Use the filter controls for:<br>
Zone Sales<br>
Start Date<br>
End Date<br>
Genre<br>
Hover over charts or bars to see tooltips with detailed information.<br>

<b>Calculated Fields and Parameters</b><br>

Parameters Used:<br>
Zone Sales: Allows the user to switch between Global, NA, EU, and JP sales zones.<br>
Start Date and End Date: Used to filter sales by time period.<br>
Genre: Dropdown parameter to filter data by game genre.<br>

Key Calculated Fields:<br>
Total Sales:<br>
SUM([Global_Sales])<br>
Calculates the total sales for selected filters.<br>

Top Genres by Sales:<br>
WINDOW_SUM(SUM([Global_Sales]))<br>
Used to rank genres.<br>

Ranked Titles:<br>
RANK(SUM([Global_Sales]))<br>
Ranks top 10 games by total sales.<br>

Sales by Year and Genre:<br>
Time series calculated by grouping data by Year and Genre fields.<br>

<b>Bug / Feature Request</b><br>
If you encounter issues or would like to suggest improvements:<br>
Email: sagar007ak@gmail.com<br>
Or raise an issue on the project repository (if applicable)<br>

<b>Authors</b><br>
Your Name: Sagar<br>
Role: Data Analyst / Tableau Developer<br>
Email: sagar007ak@gmail.com<br>
LinkedIn: www.linkedin.com/in/sagar1505<br>






