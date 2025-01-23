

# Stock Portfolio Tracker

A stock portfolio tracking tool that allows users to manage, track, and evaluate their stock investments in real-time. This application integrates with financial APIs to fetch the latest stock data and display portfolio performance.

## Features

- **Add Stock**: Add stocks to your portfolio by specifying stock symbol (e.g., AAPL, TSLA) and the quantity.
- **Remove Stock**: Remove stocks from the portfolio by specifying the stock symbol.
- **View Portfolio**: View the total value of your portfolio, individual stock performances, and changes in value over time.
- **Real-Time Stock Data**: Fetch real-time data for stock symbols, including the current price, historical data, percentage change, etc.
- **Track Performance**: Monitor the performance of individual stocks and the overall portfolio over time.

## Technologies Used

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Python (Flask/Django or Node.js with Express)
- **Database**: SQLite or PostgreSQL (for storing portfolio data)
- **APIs**: Financial APIs (e.g., [Alpha Vantage](https://www.alphavantage.co/), [Yahoo Finance API](https://www.yahoofinanceapi.com/), or [IEX Cloud](https://iexcloud.io/))
- **Authentication**: Optional (OAuth2, JWT, etc. for user login and authentication)

## Setup Instructions

### Prerequisites

- Python 3.8 or higher
- Node.js (if using for frontend or full-stack)
- API Key (for fetching real-time stock data)

### Installation


1. Install dependencies:
   - For Python:
     ```bash
     pip install -r requirements.txt
     ```

   - For Node.js (if required for frontend):
     ```bash
     npm install
     ```

2. Set up environment variables (for stock data API key):
   - Create a `.env` file in the root directory and add the following:
     ```plaintext
     STOCK_API_KEY=your-api-key-here
     ```

3. Run the application:
   - For Python (Flask/Django):
     ```bash
     python app.py
     ```
   - For Node.js:
     ```bash
     npm start
     ```

4. Access the app via your browser:
   ```plaintext
   http://localhost:5000 (or the appropriate port)
   ```

## API Integration

- To fetch real-time stock data, we use [Alpha Vantage](https://www.alphavantage.co/) or another similar API.
- The API provides endpoints like:
  - **Time Series Data**: Get the stock price for a symbol.
  - **Global Quote**: Fetch stock quote details.

### Example Request:
```bash
GET https://www.alphavantage.co/query?function=TIME_SERIES_INTRADAY&symbol=AAPL&interval=5min&apikey=YOUR_API_KEY
```

## Usage

1. **Adding a Stock**: 
   - Navigate to the "Add Stock" section.
   - Enter the stock symbol (e.g., AAPL for Apple) and the quantity of shares owned.
   - Click "Add" to update your portfolio.

2. **Removing a Stock**:
   - Navigate to the "Remove Stock" section.
   - Enter the stock symbol to remove from your portfolio.
   - Click "Remove" to update your portfolio.

3. **Viewing Portfolio**:
   - Go to the "My Portfolio" section to see your current holdings, their real-time performance, and portfolio value.

4. **Tracking Portfolio Performance**:
   - Monitor your portfolio's performance over time, including overall profit/loss and individual stock performance.

## Contributing

If you'd like to contribute to the development of this project, feel free to fork the repository and submit a pull request. Ensure that your code follows the established guidelines and is well-tested.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

