# Spotify Extended History Insights (SEHI) 📊🎧

Unlock the hidden patterns in your music journey. This toolkit transforms raw Spotify JSON data into deep analytical reports, helping you identify your "true" favorites using custom loyalty metrics.

## 🌟 Key Features

- **Data Merger:** Combines multiple `Streaming_History_Audio_*.json` files into a single master dataset.
- **20-Second Quality Filter:** Filters out accidental clicks and skipped tracks to ensure high-quality data analysis.
- **Loyalty & Skip Rate Analysis:** Calculates a unique "Loyalty Ratio" (Total Attempts vs. Meaningful Plays) to find the songs you truly love and never skip.
- **Artist Deep Dive:** Generates chronological, year-by-year reports for any specific artist in your history.
- **Top 50 Hall of Fame:** Lists your top 50 songs and artists across your entire Spotify history (2016 - Present).

## 🛠️ Installation

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/yourusername/spotify-data-analyzer.git](https://github.com/yourusername/spotify-data-analyzer.git)
    cd spotify-data-analyzer
    ```
2.  **Install Dependencies:**
    This project requires Python and the `pandas` library.
    ```bash
    pip install pandas
    ```

## 🚀 How to Use

### 1. Get Your Data
- Go to your Spotify Account -> **Privacy Settings**.
- Request **"Extended streaming history"** (Note: This may take a few days to arrive via email).
- Download and unzip the data.

### 2. Prepare the Workspace
- Copy all files named `Streaming_History_Audio_*.json` into the root directory of this project.
- **Important:** Do NOT upload your JSON files to GitHub. 

### 3. Run the Analysis
The project is designed to be used in a Jupyter Notebook (`.ipynb`) or as standalone scripts. Run the steps in order:
- **Step 1-3:** Merge files and generate the yearly master report.
- **Step 6-7:** Generate the Raw and Cleaned CSV datasets.
- **Step 9-10:** Generate your Loyalty and Skip Rate reports.

## 📊 Outputs Explained

| File | Description |
| :--- | :--- |
| `Spotify_Full_History_Dataset.csv` | Every interaction over 1 second. |
| `Spotify_Dataset_All_Time_Cleaned.csv` | High-quality data (only tracks played > 20s). |
| `Loyalty_Skip_Rate_Report.txt` | Ranking based on how often you finish a song without skipping. |
| `Spotify_Full_History_Report.txt` | Year-by-year Top 10 lists for songs and artists. |

## 🔒 Privacy First

- **Zero Data Leakage:** This script runs 100% locally on your machine.
- **No Cloud Uploads:** Your personal listening data never leaves your computer.
- **Open Source:** You can inspect the code to see exactly how your data is processed.

---
*Developed with a focus on data quality and music loyalty analysis.*