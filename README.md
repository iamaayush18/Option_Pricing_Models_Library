# Option Pricing Models Project

## What is this project about?
This project focuses on implementing two foundational models for option pricing from scratch: the Binomial Tree Model and the Black-Scholes Model. These models are critical in financial engineering and economics, providing theoretical estimates for the price of European call and put options under specific assumptions. By building these models, we aim to offer intuitive and practical tools for financial analysts, traders, and anyone interested in understanding or applying option pricing in the real world.

## Approaches

### 1. Binomial Tree Model
The Binomial Tree Model is a discrete-time model for valuing options. This model assumes that the price of the underlying asset follows a binomial process; at each step, it can move up or down by a specific factor. The model is built upon the concept of no-arbitrage and risk-neutral valuation.

- **Theory:** The model uses a binomial lattice to represent possible paths the price of the underlying asset can take over the option's life. At each node, the option value is calculated based on the payoff from moving up or down in the tree, discounted back at the risk-free rate. The process starts at the option's expiration and iterates backward to the present, yielding the option's current price.

### 2. Black-Scholes Model
The Black-Scholes Model provides a continuous-time framework for option pricing, which revolutionized the financial markets. It assumes a lognormal distribution for stock prices and derives a differential equation whose solution gives the option's price.

- **Theory:** The model is founded on the principles of hedging and no-arbitrage. It provides closed-form solutions for the prices of European call and put options on a stock that does not pay dividends. The model inputs include the stock price, strike price, risk-free rate, time to expiration, and volatility of the stock's return.

## Environment Setup

To run this project locally, you'll need to set up a Python environment with necessary libraries. Here's how to do it using Conda:

1. Install [Anaconda](https://www.anaconda.com/products/individual) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html).
2. Open your terminal (or Anaconda Prompt on Windows).
3. Create a new Conda environment: `conda create --name option_pricing python=3.8`
4. Activate the environment: `conda activate option_pricing`
5. Install the required packages: `conda install numpy pandas matplotlib scipy jupyterlab`
6. Navigate to the project directory and launch Jupyter Notebook: `jupyterlab`
7. Open the `.ipynb` files to run the project.

## Future Updates Checklist
- [ ] Automate the fetching of market data for real-time option pricing.
- [ ] Incorporate various techniques to scale Binomial Tree models to more than 10 steps.
- [ ] Implement the Monte Carlo simulation for option pricing.
- [ ] Add a GUI for interactive model parameters input and visualization.
- [ ] Extend models to price to estimate American options.
- [ ] Incorporate dividends in the Black-Scholes Model.
- [ ] Explore and integrate alternative models like the Heston model for volatility surface.
- [ ] Enhance the project documentation with more examples and use cases.

**Note:** This project is an ongoing effort by me for learning advanced financial models and demonstrating the power of programming and quantitative finance.


