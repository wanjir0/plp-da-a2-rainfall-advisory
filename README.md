# plp-da-a2-rainfall-advisory

# County Rainfall and Planting Advisory

## Project Summary

A farmer-support NGO sends SMS advice on planting windows to farmers in five counties (Nairobi, Nakuru, Kisumu, Mombasa and Machakos). The Machakos rainfall readings were typed in by hand and contained errors. This project cleans that data, analyses the monthly rainfall of all five counties with NumPy, and produces a planting advisory. The results are saved in `rainfall_summary.csv`.

## Files

- `rainfall_analysis.ipynb`: the notebook with all the code, the "Planting Advisory" and the "Data Quality Notes"
- `rainfall_summary.csv`: one row per county with `county`, `annual_total_mm`, `wettest_month`, `dry_months` and `planting_window`
- `requirements.txt`: the libraries needed to run the notebook
- `README.md`: this file

## How to Run the Notebook
1.. Open `rainfall_analysis.ipynb` in Google Colab (upload it at colab.research.google.com, or open it from GitHub or Google Drive).
2. NumPy is already installed in Colab. To install it anywhere else, run:
   ```
   pip install -r requirements.txt
   ```
3. Run all cells from top to bottom (**Runtime > Run all**).
4. The file `rainfall_summary.csv` will be created in the Colab session's file storage (see the folder icon on the left).

## Planting Advisory

- Farmers in Nairobi, Nakuru, Kisumu and Mombasa should plant in April-May, when combined rainfall is highest (between 265 mm and 420 mm).
- Farmers in Machakos should plant in November-December (278 mm combined), and because Machakos is the driest county (811 mm a year, with six dry months), drought-tolerant crops are worth considering.
- Two Machakos readings (April and September) were invalid and were estimated at 68 mm, and all results come from a single year of data, so the advice should be checked against more years before it is sent out.
