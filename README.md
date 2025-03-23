# ATAIX USDT Trading Bot

## Overview
This Python-based automated trading bot interacts with the ATAIX exchange API. It retrieves the available USDT balance, finds suitable trading pairs, and places limit buy orders at predefined price levels (-2%, -5%, -8% from the highest bid). The bot logs all executed orders in a JSON file.

## Features
- Fetches USDT balance from the ATAIX API
- Identifies trading pairs with USDT as the quote currency
- Retrieves the highest bid price for a selected pair
- Places limit buy orders at strategic price levels
- Logs executed orders into a JSON file for record-keeping

## Requirements
- Python 3.7+
- `requests` library

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/ataix-trading-bot.git
   cd ataix-trading-bot
   ```
2. Install dependencies:
   ```sh
   pip install requests
   ```
3. Set up your API key:
   - Replace the `API_KEY` value in `main.py` with your ATAIX API key.

## Usage
Run the script:
```sh
python main.py
```

## Configuration
You can modify the following parameters in `main.py`:
- `API_KEY`: Your ATAIX API key
- `BASE_URL`: API base URL
- `price levels`: Adjust price deviation percentages for buy orders
- `num_orders`: Number of orders placed per trading session

## Example Output
```
Available balance: 1.916057 USDT
Selected trading pair: TRX/USDT
Highest bid price: 0.230000 USDT
Order 1 placed: {order details}
Order 2 placed: {order details}
Orders saved to orders.json
```

## License
MIT License. See `LICENSE` for details.

## Disclaimer
This bot is for educational and research purposes only. Use at your own risk.
