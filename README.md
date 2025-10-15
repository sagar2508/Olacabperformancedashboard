# Ola Data Dashboard

**Project:** Ola Data Dashboard

**File included:** `Ola Data Dashboard.pbix`

## About

A Power BI report and data model that visualizes ride-sharing metrics and business KPIs for the Ola dataset. The dashboard includes interactive visualizations, filters, and a data model intended to help stakeholders monitor performance, operations, and user trends.


## Key Features

* Executive summary page with top-level KPIs (total rides, revenue, active drivers, active users)
* Time-series analysis (daily/weekly/monthly trends)
* Geographic visualizations (city/region level maps)
* Customer segmentation and cohort analysis
* Operational metrics (average trip time, cancellation rate, utilization)
* Interactive slicers for date ranges, regions, and vehicle types

---

## Files & Structure (recommended)

```
/ (root)
├─ Ola Data Dashboard.pbix        # Main Power BI Desktop file (this repo)
├─ data/                         # (optional) raw CSVs / extracts (NOT included)
├─ docs/                         # screenshots, data dictionary, additional docs
└─ README.md                     # Project readme (this file)
```

---

## Prerequisites

* [Power BI Desktop](https://powerbi.microsoft.com/) (recommended latest version) to open and edit the `.pbix` file.
* If you plan to publish the report to Power BI Service, you will need a Power BI account (Pro or Premium per your organization needs).

---

## How to open & view

1. Download or clone this repository to your local machine.
2. Open `Ola Data Dashboard.pbix` with Power BI Desktop.
3. If the data model has broken connections, update the data source credentials in **Home → Transform data → Data source settings**.

### Typical workflows

* **Edit visuals / data model:** Open in Power BI Desktop, make changes, and save the `.pbix` file.
* **Refresh data locally:** Use the **Refresh** button in Power BI Desktop after ensuring the data sources are reachable and credentials are set.
* **Publish to Power BI Service:** In Power BI Desktop: `File → Publish → Publish to Power BI` and choose the workspace.

---

## Data & Connections

The `.pbix` file contains the data model and visualizations but not the underlying raw data extracts. Common data sources used with dashboards like this are:

* CSV/Excel extracts (e.g., `data/trips.csv`)
* SQL databases (Azure SQL, SQL Server, MySQL)
* Cloud storage (Azure Blob, S3)

**Important:** If you open the file and visuals appear broken or missing data, you likely need to re-point the queries to your local dataset or update credentials. To update connections:

1. `Home → Transform data → Data source settings`
2. Select the data source → `Change Source...` or `Edit Permissions...`

You can also open **Transform data → Power Query** to view each query and where it expects data to be located.

---

## Suggested README additions (please fill in)

* Data dictionary (table and column descriptions)
* Exact data sources & connection strings (replace sensitive credentials with instructions)
* Screenshots of the dashboard pages (place in `docs/` and link them here)
* Schedule / refresh instructions if using Power BI Service (gateway details)

---

## Publishing & Embedding

* Publish to Power BI Service from Power BI Desktop using your account.
* To schedule refreshes, configure a data gateway and set refresh schedule in the Power BI Service workspace.
* To embed in a web portal or internal site, use Power BI embedding options in the service (requires proper licensing).

---

## Contributing

If you want to contribute changes to the dashboard (improved visuals, new measures, or updated model):

1. Fork this repository.
2. Add your updated `.pbix` file (rename with a version like `Ola Data Dashboard v1.1.pbix`).
3. Open a Pull Request describing the changes and screenshots of the updated visuals.

---

## Troubleshooting

* **Broken visuals / missing data:** Check data source settings and credentials.
* **Slow performance:** Consider optimizing the data model (remove unused columns, reduce granular history, use star schema) and use aggregations.
* **Publish errors:** Ensure your Power BI account has the correct permissions for the chosen workspace and licensing.

---

## License

Specify a license for this repository (e.g., MIT). Add a `LICENSE` file at the root.

---

## Contact / Author

If you have questions, changes, or want help improving the report, add your contact information here:

* **Author:** *Your Name*
* **Email:** *[your.email@example.com](mailto:your.email@example.com)*

---

## Changelog

* **v1.0** — Initial upload of `Ola Data Dashboard.pbix`.

---

**Want this README customized?** I can add a data dictionary, example screenshots, or exact connection instructions — tell me what details you want included and I will update the README.
