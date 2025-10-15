# Sales Summary Dashboard

This project provides a simple web-based dashboard to visualize product sales data. It allows users to view total sales per product, convert sales figures to different currencies, and filter sales by region.

## Features

- **Product Sales Listing**: Displays a table of each product with its aggregated total sales.
- **Currency Conversion**: Select from various currencies to view sales totals in your desired denomination. Exchange rates are sourced from `rates.json`.
- **Region Filtering**: Filter the sales data to see totals for specific geographic regions.
- **Responsive Design**: Built with Tailwind CSS for a modern, mobile-friendly interface.

## Project Structure

- `index.html`: The main HTML file containing the dashboard layout, styling (Tailwind CSS), and all application logic (JavaScript).
- `data.csv`: A CSV file containing raw sales transaction data. It's expected to have columns like `Product`, `Region`, and `SalesAmount`.
- `rates.json`: A JSON file providing exchange rates for different currencies, relative to a base currency (e.g., USD).
- `README.md`: This file, providing an overview of the project.
- `LICENSE`: The MIT License for this project.

## How to Run

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd sales-summary-dashboard
    ```
2.  **Ensure data files are present:** Make sure `data.csv` and `rates.json` are in the project root directory.
3.  **Open `index.html`:** Simply open the `index.html` file in your web browser. There is no server-side component required.

## Data Formats

### `data.csv`

Expected format for `data.csv` (example):

```csv
Product,Region,SalesAmount
Laptop,North America,1200.50
Mouse,Europe,25.00
Keyboard,Asia,75.20
Laptop,Europe,1500.00
```

### `rates.json`

Expected format for `rates.json` (example, with USD as base):

```json
{
  "USD": 1.0,
  "EUR": 0.85,
  "GBP": 0.75,
  "JPY": 110.25
}
```

## Technologies Used

-   **HTML5**: Structure of the web page.
-   **Tailwind CSS**: Utility-first CSS framework for styling.
-   **JavaScript (Vanilla)**: For data fetching, processing, filtering, and dynamic updates.

## Contributing

Feel free to fork this repository, open issues, or submit pull requests. All contributions are welcome!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.