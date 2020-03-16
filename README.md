# MCTS for Dynamic Pricing
This project is pertinent to dynamic pricing for the fashion retail industry by using Monte Carlo Tree Search with UCB1 Strategy. For simplification, this demo version will focus on strategic pricing decision for 3 specific SKUs in a boutique store.

K-Fashion is a boutique store for women’s fashion apparel located in a big shopping mall at the Causeway Bay. The store is targeting young female white-collar who care less about brand but more about fashion and price. 

For the next three-month season, K-Fashion has ordered 200 different stock keeping units1 (SKUs) from a foreign supplier. Due to the long production and order lead time, K-Fashion can place the order only once. Given the large store traffic at Causeway Bay, the store ordered 10 pieces for each SKU. 

To simplify the analysis, assume that the demand for each SKU is independent and statistically identical, i.e., each of the three SKUs has its own buyers and cannot substitute each other. Buyers for each SKU arrive randomly. According to past experience, suppose at most one buyer (i.e., 0 or 1) will show up during a day. If a buyer shows up, his or her valuation for the SKU will be random and in general the value decreases over time.If a buyer shows up but finds that the price is higher than her valuation, then there is a chance that she will come back during the last week of the season with a new, random valuation. 
 
The challenge for K-Fashion is how to maximize the total revenue, given the fixed amount of inventory over the next three months or 12 weeks. Any unsold inventory after the twelfth week will be discarded with zero salvage value. 

The goal is to focus on the pricing of three SKUs: A, B, and C, the sales of which are independent of other SKUs. Same price should be set for all the three SKUs as they differ only in color or size. The price can only be adjusted every Monday. Pick a price from the set: {999, 899, 799, 699, 599, 499, 399, 299, 199, 99}.
