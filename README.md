# Sales Performance Dashboard (First Project)

An Excel-based sales analysis covering **2019-2024**, published as an interactive web dashboard.
Open `index.html` in any browser (no install, no internet needed), or host it free with GitHub Pages.

## Key figures

| Metric | Value |
|---|---|
| Transactions (after cleaning) | 51,116 |
| Total sales | $1.663 billion |
| Total profit | $541.0 million |
| Profit margin | 32.5% |
| Customers | 9,932 |
| Products | 28 across 7 categories |

## What the dashboard shows

- **Revenue**: monthly revenue, revenue by product category, monthly profit trend, revenue share by country and by age group
- **Products**: category share, monthly units sold, 5 best and 5 under-performing products
- **Customers**: top customers by average order value, revenue by age group, yearly revenue

## Repository structure

```
first-project-sales-dashboard/
├── index.html                 # the interactive dashboard (self-contained)
├── README.md
├── .gitignore
├── data/
│   ├── cleaned_sales_data.csv # cleaned transactions used for the analysis
│   └── dashboard_data.json    # aggregated numbers behind each chart
└── excel/
    └── First_Project.xlsx     # original workbook: Raw Data, Cleaned, Pivot Table, dashboards
```

## Data cleaning (Excel)

The `Raw Data` sheet had 52,021 rows. In the `Cleaned` sheet:

- Country names standardised (extra spaces, upper/lower-case variants such as `GERMANY`, `mexico`)
- Ages stored as text (for example `32 yrs`) converted to numbers
- Invalid month numbers rebuilt from the transaction date
- Missing values and duplicate transactions removed
- Age groups added: Young Adult (up to 27), Adult (28-35), Old Adult (36-43), Elders (44-51), Senior (52-60)

## Tools

Microsoft Excel (Power Query-style cleaning, pivot tables, dashboards) and plain HTML/CSS/JavaScript for the web version.

## Publish it with GitHub Pages

1. Create a new repository on GitHub and upload the contents of this folder.
2. Go to **Settings > Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
4. After a minute your dashboard is live at `https://<your-username>.github.io/<repository-name>/`.

## Author

Add your name and program details here.
