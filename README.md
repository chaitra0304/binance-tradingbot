**Binance Futures Testnet Trading Bot
Overview

This is a Python-based CLI trading bot that places MARKET and LIMIT orders on Binance Futures Testnet (USDT-M).
It is designed with a clean structure, input validation, logging, and error handling.

Features
1. MARKET and LIMIT orders
2. Supports BUY and SELL sides
3. CLI-based input using argparse
4. Input validation
5. Structured logging (requests, responses, errors)
6. Exception handling for API and network issues

Setup
1. Clone the repository:
git clone https://github.com/your-username/binance-trading-bot.git
2. Install dependencies:
pip install -r requirements.txt
3. Create a .env file:
API_KEY=your_api_key
API_SECRET=your_api_secret

Usage
Market Order
python cli.py --symbol BTCUSDT --side BUY --type MARKET --quantity 0.001

Limit Order
python cli.py --symbol BTCUSDT --side BUY --type LIMIT --quantity 0.001 --price 60000

Sample Output
Order summary is displayed in the terminal
API response includes:
orderId
status
executedQty
avgPrice (if available)
Logging

All requests, responses, and errors are logged in: app.log

Assumptions
Uses Binance Futures Testnet (USDT-M)
API keys are configured via .env
LIMIT orders use GTC (Good Till Cancelled)

Notes
.env file is excluded from the repository for security
Testnet environment is used (no real funds involved)
