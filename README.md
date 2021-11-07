# Arbitrage
This project will simulate the currency arbitrage using Bellman-Ford algorithm

# Example of currency Arbitrage
Suppose the currency rate are shown as below:  
1 USD buys 0.82 Euro  
1 Euro buys 129.7 Yen  
1 Yen buys 12 Turkish Lira  
1 Turkish Lira buys 0.0008 USD  

usd -> euro -> yen -> lira -> usd    
Finally, 1 usd -> 1.02 usd(0.82 · 129.7 · 12 · 0.0008 ≈ 1.02)  


# currency Arbitrage as negative cycles 
Using R(ci, cj) represents i unit of ci can buy how many unit of cj.  
We want to find R(c1, c2) * R(c2, c3) * ... * R(ck, c1) > 1.  
We can use math to convert it into negative cycles in the following way:  

  ![Alt text](https://github.com/SouthernPark/Arbitrage/blob/main/img/p1.PNG)  
  
  ![Alt text](https://github.com/SouthernPark/Arbitrage/blob/main/img/p2.PNG)  
