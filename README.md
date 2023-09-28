# Portfolio-optimization-using-Genetic-algorithm

Portfolio optimization is crucial for investors seeking to maximize their returns while minimizing risks. Genetic algorithms (GA) are powerful optimization tools that can solve this problem. This method is designed to find the optimal combination of assets that maximizes the return on investment while adhering to certain constraints, such as the maximum allowable investment in any given asset or sector

Suppose we have identified N financial assets that we wish to invest in, such as stocks, funds, bonds, or ETFs. Each asset has a historical return, which refers to the relative price difference between two periods, such as days, weeks, or months. Our objective is to construct an investment portfolio that comprises a mixture of several assets, and allocate a fraction x of total capital to each asset, which is known as the weight. The aim of portfolio optimization is to determine the optimal weights for each asset that maximizes returns and minimizes risk while adhering to certain constraints.

### Given Data:
Monthly Closing Stock values of HDFC, ITC, L&T, M&M, Sun Pharma and TCS from June 2015 to June 2018.

### Theoretical Approach for the Problem used:
Firstly, the data for the monthly closing stock values are combined into a single dataframe. Historical returns for periods ranging from 3 to 36 months are then calculated for each stock. The next step is to define the genetic algorithm terms - Gene and Chromosome. Gene is a scalar, which represents a fraction of the total capital assigned to a stock, whereas a Chromosome is a 1D array consisting of a set of genes, i.e., fractions of total capital assigned to each stock. It is essential to ensure that the sum of each chromosome is equal to one.

After defining the Gene and Chromosome, the next step is generating an Initial Population, a 2D array consisting of randomly generated chromosomes. The fitness function is then defined, which calculates the Sharpe ratio, S. The Sharpe ratio is a measure that quantifies the portfolio's performance by maximizing return and minimizing risk simultaneously. It is computed as the difference between the portfolio return and the risk-free rate, divided by the standard deviation of the returns. The fitness function uses the mean portfolio return, risk-free rate, and the standard deviation of the portfolio return to calculate the Sharpe ratio.

We will also compare our returns with that of the MPT (Modern Portfolio Theory) and see how our modified optimization gives better returns for reduced risks.

#### References:
1. https://www.researchgate.net/publication/286952225_A_heuristic_crossover_for_portfolio_selection
2. https://pdfs.semanticscholar.org/9888/061ea3326ff9b41c807ed21f0c10463b7879.pdf
3. https://www.math.kth.se/matstat/seminarier/reports/M-exjobb12/121008.pdf


