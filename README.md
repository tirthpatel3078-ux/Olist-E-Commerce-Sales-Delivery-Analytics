# Olist E-Commerce Sales & Delivery Analytics

Combines Olist's Brazilian e-commerce data into clean order- and item-level datasets,
analyzes sales, delivery, product, and customer-review trends, and exports results for
Power BI.

## Resume description
- Investigated how delivery reliability relates to customer experience by comparing delivery times and late orders with review scores, helping identify fulfillment issues worth addressing.
- Combined Olist's order, item, payment, review, customer, and product records with pandas to create consistent order- and item-level views for business analysis.
- Explored when and where sales occur and which product categories contribute most, then prepared clear visualizations and Power BI-ready tables for further decision-making.

**Dataset:** https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

## How to run
1. Use Python 3.11 or newer and create a virtual environment in the project folder:
   ```powershell
   python -m venv .venv
   .\.venv\Scripts\Activate.ps1
   python -m pip install -r requirements.txt
   ```
2. Download the dataset zip from Kaggle and extract the CSV files. Put them in the project
   folder (beside `olist.py`) or in `data/raw/`.
3. Run the script:
   ```powershell
   python olist.py --data . --out output
   ```
   If the CSV files are in `data/raw/`, use `python olist.py` instead.
4. To use the notebook, run `jupyter notebook`, open `Olist_EDA.ipynb`, and select Run All.

Outputs are saved in `output/` (figures, summary CSVs and `powerbi_ready/`).
