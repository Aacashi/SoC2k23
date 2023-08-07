Task 3 alphas:
1. (-1 * ts_max(rank(correlation(rank(volume), rank(vwap), 5)), 5)) 
2. (((((delay(close, 20) - delay(close, 10)) / 10) - ((delay(close, 10) - close) / 10)) < (-1 * 0.05)) ? 1 : ((-1 * 1) * (close - delay(close, 1)))) 
3. ((((-1 * ts_min(low, 5)) + delay(ts_min(low, 5), 5)) * rank(((sum(returns, 240) - sum(returns, 20)) / 220))) * ts_rank(volume, 5)) 
4. (-1 * delta((((close - low) - (high - close)) / (close - low)), 9)) 
5. ((-1 * ((low - close) * (open^5))) / ((low - high) * (close^5))) 
