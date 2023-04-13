# Personal Finance Planner

This Python script helps users to visualize their savings and investments to make better financial decisions. The application fetches current cryptocurrency prices and stock prices, calculates the value of the user's holdings, and runs a Monte Carlo simulation to project the value of the user's stock and bond investments over 30 years.

## Dependencies

- pandas
- os
- requests
- dotenv
- alpaca_trade_api
- MCForecastTools

## Usage

1. Install the required dependencies.

2. Set up a `.env` file with the following variables:

    * ALPACA_API_KEY=<your_alpaca_api_key>
    * ALPACA_SECRET_KEY=<your_alpaca_secret_key>

3. Update the following variables in the script with your current assets and investments:

    * my_btc
    * my_eth
    * my_agg
    * my_spy
    * monthly_income

4. Run the script:

    * python personal_finance_planner.py

5. The script will display the current value of your cryptocurrency and stock holdings, a pie chart showing the composition of your savings, and information about your emergency fund.

6. The script will also run a Monte Carlo simulation to forecast the cumulative returns of a 60% stocks (SPY) and 40% bonds (AGG) portfolio over the next 30 years. It will provide a range of possible outcomes for an initial investment of $20,000 and $30,000.

## Output

- The current value of your cryptocurrency and stock holdings
- A pie chart showing the composition of your savings
- Information about your emergency fund
- A line plot of 500 simulated cumulative return paths for a 60% stocks (SPY) and 40% bonds (AGG) portfolio over the next 30 years
- A histogram plot of the distribution of cumulative returns
- A range of possible outcomes for an initial investment of $20,000 and $30,000 over the next 30 years, with a 95% confidence interval

## Disclaimer

This script is for informational purposes only and should not be considered financial advice. The results of the Monte Carlo simulation are based on historical data and should not be considered indicative of future performance. Always consult a financial advisor before making investment decisions.
