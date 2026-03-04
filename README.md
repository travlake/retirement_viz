# Retirement Portfolio Monte Carlo Simulator

Interactive browser-based tools for visualizing retirement portfolio risk using bootstrap Monte Carlo simulation with historical U.S. market returns (July 1926 – December 2024).

Built live in class as a demo of [Claude Code](https://docs.anthropic.com/en/docs/claude-code).

## Tools

### `index.html` — Retirement Drawdown Simulator
Simulates portfolio depletion during retirement. Configure starting balance, monthly withdrawal, withdrawal growth rate, horizon, and number of simulations. Displays a fan chart (10th–90th and 25th–75th percentile bands with median) and ruin probability.

### `saving.html` — Retirement Savings Simulator
Simulates portfolio accumulation before retirement. Configure current savings, monthly contributions, contribution growth, stock/bond allocation, horizon, and number of simulations. Fan chart shows percentile bands plus a dashed line for cumulative contributions.

### `saving_final.html` — Extended Savings Simulator
A more detailed version developed separately (not built live in lecture). Features include historical portfolio path overlay, simulation path spaghetti plot, log/linear scale toggle, and detailed return statistics (annualized mean/std dev, skewness, kurtosis, max drawdown). Fetches data from a hosted CSV rather than embedding it.

## Data

`mktrf.csv` contains monthly U.S. market excess returns (`mktrf`) and risk-free rates (`rf`) from the Fama-French data library, July 1926 through December 2024 (1,182 months).

## Usage

Open any `.html` file directly in a browser. No build step or server required (`saving_final.html` fetches its data from a remote URL, so it does need internet access).
