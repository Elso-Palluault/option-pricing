# Option Pricing: Black-Scholes and Monte Carlo

Pricing European call and put options with the Black-Scholes formula and by Monte Carlo simulation of a geometric Brownian motion, and analysing the Greeks, in Python (NumPy, pandas, SciPy, matplotlib).

**Status: complete.**

## Steps
- [x] Step 1: Payoffs of a call and a put at maturity
- [x] Step 2: Black-Scholes prices and put-call parity check
- [x] Step 3: Simulation of stock prices with a geometric Brownian motion, martingale check of the discounted price
- [x] Step 4: Monte Carlo pricing, confidence intervals and convergence
- [x] Step 5: Delta, gamma and vega (closed formulas and bump and reprice), sensitivity of the price to volatility

## Key findings
- For an at-the-money option (stock at 100, strike 100, one year, 3% rate, 20% volatility), the call is worth 9.41 and the put 6.46, and put-call parity holds exactly.
- The discounted mean of 10,000 simulated prices at maturity (99.81) is close to today's price (100), as expected under the risk-neutral measure.
- With 100,000 simulations, Monte Carlo prices are within a few cents of Black-Scholes; the standard error falls with the square root of the number of simulations (0.14 with 10,000, 0.014 with 1,000,000).
- The at-the-money call has a delta of 0.60 and a vega of 0.39 per volatility point; gamma and vega peak around the strike.

Educational project.
