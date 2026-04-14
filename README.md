⚡ Indian Electricity Trends Dashboard (2019–2024)

📊 Project Overview

This project presents an interactive Power BI dashboard that analyzes electricity generation across India from 2019 to 2024.
It provides both overall trends and state-wise insights, helping users understand energy patterns, growth, and distribution.

🎯 Objectives

Analyze electricity generation trends over time
Compare state-wise performance
Identify top and lowest electricity-producing states
Understand energy source distribution
Provide interactive and insightful visualizations

📁 Dataset

Source: Ember Energy Dataset
Data includes:
State-wise electricity generation
Energy types (Coal, Renewable, Fossil, etc.)
Year-wise values
Units (GWh, %, MW, etc.)
🛠 Tools & Technologies
Power BI – Dashboard creation
DAX (Data Analysis Expressions) – Measures & KPIs
Excel / CSV – Data source
Data Modeling & ETL

📌 Key Features

🔹 Overview Dashboard

Total Electricity Generation KPI
Growth Analysis
Year-wise Trends
Energy Source Distribution (Pie Chart)
Top 5 Electricity Producing States

🔹 State-wise Analysis

Interactive India Map (state-level insights) 🗺️
Top & Lowest State Identification
Decomposition Tree (AI-based analysis) 🌳
State-wise Generation Comparison
Dynamic filters (Year & Unit)

📈 Key Insights

Maharashtra is the top electricity producing state
Chandigarh is the lowest electricity producing region
Electricity generation shows a steady growth trend from 2019–2024
Fossil fuels dominate, but renewable energy is increasing 🌱

🧠 DAX Measures Used

Total Generation = SUM('Table'[Energy_Value])

Average Generation = AVERAGE('Table'[Energy_Value])

Top State = 
VAR TopStateTable =
    TOPN(1, VALUES('Table'[State]), [Total Generation], DESC)
RETURN
    CONCATENATEX(TopStateTable, 'Table'[State], ", ")

Lowest State = 
VAR BottomStateTable =
    TOPN(1, VALUES('Table'[State]), [Total Generation], ASC)
RETURN
    CONCATENATEX(BottomStateTable, 'Table'[State], ", ")

🚀 How to Use

Download the .pbix file
Open in Power BI Desktop
Use slicers to filter:
Year
Unit (GWh recommended)
Interact with visuals for deeper insights

📬 Contact

Feel free to connect for feedback or collaboration!

⭐ If you like this project, don’t forget to star the repository!
