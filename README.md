# Multiple-Underlying Capped Accumulated Return Call Option

A pricing model is presented for capped-accumulated-return-call (CARC) with multiple underlyings. At each reset date, a weighted stock price is calculated.  These weighted stock prices are used to compute returns.

Let   be N stocks in a given basket,   be the price process of the jth stock and  , and   be a set of reset dates and   be a payoff settlement date.  The CARC with the multiple underlyings   is a European type derivative security whose matured payoff at the settlement date is given by

	 	(1)

where   is the global floor (strike) of the return rate, N is the notional principal, and   is capped-accumulated-return and defined as

	 	(2)

where   is the capped return-rate for each period explained as follows.  Define the actual period return-rate as
				 ,	(3)

Where

	 .	(4)

Here   are the weights and

	 .	(5)

Then we define

	 ,	(6)

where c is the cap.

Let t be the current value date, then the current value of this CARC can be written as

	 	(7)

where   is the discounting factor at the value date.  The above formula is in a world that is forward risk-neutral with respect to a specific currency  .  

As a result, the notional principal N is measured in the currency  , and the discounting factor should be calculated by a   zero curve (ref. https://finpricing.com/lib/IrCurveIntroduction.html) given at the value date.  If the underlying asset is measured in another currency  , assuming the option is a Quanto type transaction, the governing price dynamics of the underlying asset in the risk-neutral world of   should be written as

	 	(8)

where   is the short rate of  , q is the dividend yield of the asset,   is the volatility of the asset price,   is the volatility of the exchange rate between   and  ,   is correlation coefficient between the asset price and the exchange rate, and   is the Wiener process.  All these parameters are assumed deterministic.





