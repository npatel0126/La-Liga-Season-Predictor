# ⚽ La Liga Data Explorer 📊📈  
A data scraping and analysis project focused on Spain’s La Liga football league. This project collects real-time match and team data from the web, cleans and processes it, and performs insightful analytics to uncover patterns in team performance across the league. Utilizing the data from the past 10 seasons the machine learning model aims to predict the winner of this season, UEFA competition qualifiers, and teams that will be relegated to the second division this season. 

---

## 📸 Preview  
> ![image](https://github.com/user-attachments/assets/bd639fb1-8038-4ac4-bede-614c1132609e)

---

## 💡 Features  

### 📥 Data Scraping  
- Automatically fetches latest La Liga standings from web sources  
- Extracts relevant columns like: Team, Games Played, Wins, Draws, Losses, Goals Scored/Conceded, and Points Per Game
- Saves data in a structured `.csv` format

### 🧹 Data Cleaning  
- Handles missing or malformed entries  
- Normalizes team names and formats numbers  
- Removes unnecessary columns to keep dataset clean and efficient

### 📊 Data Analysis  
- Calculates and compares total wins, points, and goal differences  
- Highlights top-performing and underperforming teams  
- Generates bar plots and summaries using `matplotlib`
- Predicting the winner of 2024-2025 season, qualifiers for UEFA Competitions and teams that will get relegated to the second division in Spain

---

## 🚀 How to Use  

### 1️⃣ Scrape the Data  
Open and run `data_scrapping.ipynb`  
- Grabs current La Liga table from the web  
- Saves it as `la_liga_data.csv` for analysis

### 2️⃣ Analyze the Data  
Open and run `data_analysis.ipynb`  
- Reads the `.csv` file  
- Cleans and formats the data  
- Performs statistical analysis and creates visual insights  

---

## 📁 File Breakdown  

### `data_scrapping.ipynb`  
- Uses `pandas`  
- Extracts HTML table data  
- Converts to DataFrame and exports to CSV  

### `la_liga_data.csv`  
- Stores cleaned La Liga match data  
- Columns: `Team`, `Games Played`, `Wins`, `Draws`, `Losses`, `Goals Scored`, `Goals Against`, `Goal Difference`, `Points Per Game`

### `data_analysis.ipynb`  
- Reads and processes the `.csv`  
- Uses `pandas`, `matplotlib`, and `scikit-learn`  
- Displays graphs like:
  - Top 3 ranks
  - Points per game average 

---

## 🔥 Key Takeaways  
📌 Based on the analysis of the past 10 seasons, FC Barcelona has a 70.83% chance of winning the league this season followed by Real Madrid and Atlético Madrid. 
📌Teams that will see European Competitions next season:
    - Champions League 
        * Barcelona 
        * Real Madrid 
        * Atlético Madrid
        * Athletic Club 
        * Villarreal
    - Europa League 
        * Betis 
        * Mallorca
    - Coference League 
        * Rayo Vallecano 
📌Teams that have the potential of being relegated this season:
    * Leganés
    * Las Palmas
    * Valladolid

---

## 📦 Libraries Used  
- `pandas`  
- `numpy`  
- `matplotlib`  
- `scikit-learn`  
