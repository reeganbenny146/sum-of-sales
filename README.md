# Sales Dashboard

This is a simple, single-page web application designed to fetch sales data from a `data.csv` file, calculate the total sales, and display it on a responsive dashboard.

## Features

*   **Data Fetching:** Automatically fetches `data.csv` from the project root.
*   **Sales Aggregation:** Parses the CSV and sums values from the 'sales' column.
*   **Responsive Design:** Built with Tailwind CSS to ensure a great user experience on all devices.
*   **Error Handling:** Provides user-friendly messages if the data cannot be loaded or processed.

## Project Structure

```
./
├── index.html
├── data.csv
└── README.md
└── LICENSE
```

## `data.csv` Format

The application expects a CSV file named `data.csv` located in the same directory as `index.html`. The CSV *must* include a header row, and one of the headers *must* be `sales` (case-insensitive).

**Example `data.csv`:**

```csv
product,sales,region
Laptop,1200.50,North
Mouse,25,North
Keyboard,75.99,South
Monitor,300,East
Webcam,50,West
Laptop,1500,South
```

## Setup and Usage

To run this application, you only need a web server (even a simple local one) to serve the `index.html` and `data.csv` files.

### Local Setup (Recommended)

1.  **Save the files:**
    *   Save the `index.html` content to `index.html`.
    *   Save your sales data (following the format above) to `data.csv`.
    *   Save this `README.md` content to `README.md`.
    *   Save the `LICENSE` content to `LICENSE`.

2.  **Serve files:** You can use a simple Python HTTP server:
    ```bash
    python3 -m http.server
    # Or for Python 2.x
    python -m SimpleHTTPServer
    ```
    Navigate to `http://localhost:8000` (or the port indicated by the server) in your web browser.

    Alternatively, if you have Node.js installed, you can use `http-server`:
    ```bash
    npm install -g http-server
    http-server .
    ```
    Then open `http://localhost:8080` (or default port) in your browser.

### Direct Opening (Limited Functionality)

You can also open `index.html` directly in your browser (`file:///path/to/your/project/index.html`). However, due to browser security restrictions (CORS), `fetch` requests for local files (`data.csv`) might not work. Using a local HTTP server is the recommended approach.

## Technologies Used

*   **HTML5:** Structure of the web page.
*   **Tailwind CSS:** For all styling and responsive design.
*   **JavaScript (ES6+):** For fetching, parsing, and displaying data.

## License

This project is open-source and available under the MIT License. See the `LICENSE` file for more details.
