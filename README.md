# Dodgy Dave's Stock Predictions

A fun, tongue-in-cheek web application that generates humorous AI-powered stock prediction reports. Add up to 3 stock tickers and get "super accurate" predictions with Dodgy Dave's signature style!

> ⚠️ **Disclaimer**: This is not real financial advice! Always correct 15% of the time! 😜

## Features

- Add up to 3 stock tickers for analysis
- Fetches real stock data from Polygon.io API (past 3 days)
- Generates entertaining AI-powered stock prediction reports
- Clean, responsive UI with loading states
- Humorous, exaggerated reporting style

## Tech Stack

- **Vite** - Build tool and dev server
- **Vanilla JavaScript** - ES6 modules
- **Polygon.io API** - Stock market data
- **OpenAI API** (via Cloudflare Worker) - AI report generation
- **CSS3** - Custom styling with Google Fonts

## Setup

1. **Install dependencies:**
   ```bash
   npm install
   ```

2. **Set up environment variables:**
   Create a `.env` file in the root directory:
   ```
   POLYGON_API_KEY=your_polygon_api_key_here
   ```

3. **Start the development server:**
   ```bash
   npm run dev
   ```

4. **Build for production:**
   ```bash
   npm run build
   ```

## Usage

1. Enter a stock ticker symbol (e.g., `MSFT`, `TSLA`, `AAPL`)
2. Click the add button to add it to your list
3. Add up to 3 tickers total
4. Click "Generate Report" to fetch stock data and generate your prediction
5. Read Dodgy Dave's entertaining analysis!

## Project Structure

```
dodgy-dave-stock-predictions/
├── index.html          # Main HTML structure
├── index.js            # Application logic
├── index.css           # Styling
├── vite.config.js      # Vite configuration
├── utils/
│   └── dates.js        # Date utility functions
└── images/             # Logo and UI assets
```

## API Dependencies

- **Polygon.io API**: Requires an API key for stock data fetching
- **OpenAI API Worker**: Cloudflare Worker endpoint at `https://openai-api-worker.guil-9d2.workers.dev`

## Notes

- The app fetches stock data for the past 3 days (configurable in `utils/dates.js`)
- Reports are limited to 150 words and styled with humorous, exaggerated language
- The app handles errors gracefully with user-friendly messages
