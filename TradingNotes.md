# Day Trading Opinionated
## About Me

I build my approach around a mix of **market understanding** and **data-driven validation**:  

- Develop a working knowledge of the concepts below.  
- Use algorithms to **backtest trading theses** and validate ideas.  
- Engineer features and apply **machine learning models** to identify the most impactful factors and estimate trading probabilities.  

## A Note on Opinions and Levels

The concepts here - **market structure**, **footprint charts**, **volume profile**, and **options flows** - are all frameworks to help build opinions about market direction.  
They can give you an edge by showing how other participants may be positioned, but they are **not guarantees**.

Markets are complex, and even the strongest levels or theses can break without warning. Dealer hedging flows shift, economic data surprises, and sentiment can flip quickly.  
Treat these ideas as tools to **frame probabilities**, not as certainties.

### Stay Flexible
- Have a thesis, but accept when price action proves it wrong.  
- Respect that levels fail, sometimes dramatically.  
- Adapt instead of clinging to a broken opinion.  

In short: **use these frameworks to guide decisions, not to predict with certainty.**


## Understanding Market Structure

- **Key Price Levels:** Identify important prices where the market often changes direction.  
- [Understanding Market Structure for Trading](https://youtu.be/sgAnVR6RSDg?si=Z8zKjSa3pxBMW84U)

---

## Footprint Charts

- **Delta:** Shows whether there's more buying or selling.  
- **Imbalances:** Highlights when buyers or sellers are overpowering the market.  
- **Absorption:** Indicates large orders being absorbed at certain prices.  
- **Exhaustion:** Signals slowing activity, which might mean a trend is about to change.  
- [Understanding Footprint Charts](https://www.youtube.com/watch?v=6lRy3QdLciM)

---

## Volume Profile

- **Market Participation Insight:** Understand where the majority of trading activity occurs at specific price levels.  
- **Key Levels:** Identify high-volume nodes (areas of significant interest that may act as stronger support or resistance) and low-volume nodes (potential areas where price will quickly break or reject).  
- [Volume Profile Trading](https://www.youtube.com/watch?v=vVMJa7dyYWE)

---

## Options and Their Influence on the Underlying

Even if you don’t trade options, it's important to know that options can influence the underlying price. Understanding this helps you possibly anticipate price movements based on how much options market makers (dealers) are exposed to.  
Even though this is a high-level overview, these topics are more advanced and you don't need to know them in detail. You just need to basically understand that it can impact the market because the dealer may suppress or amplify the moves based on their exposure.

- [How Options Move the Markets](https://youtu.be/0oJqC9QK-I0?si=YM_tOxYeLYYIEnuY)  
- [Understanding GEX](https://www.youtube.com/watch?v=xWLx3vPfe7U)  
- [Understanding VEX](https://www.youtube.com/watch?v=PUlVpSJJdfw)  
- [Understanding CEX](https://www.youtube.com/watch?v=lUXhZ1asBRQ)

### Key Terms

- **Gamma:** Measures how quickly an option’s sensitivity (delta) changes as the underlying price moves. High gamma means delta changes rapidly.  
- **Vanna:** Measures how an option’s delta changes when the underlying volatility changes. High vanna means delta is very sensitive to volatility.  
- **Charm:** Measures how an option’s delta changes over time, often decreasing as the option gets closer to expiration.  

### Hedging Options

- **Initial Delta Hedge:** When dealers trade options, they buy or sell the underlying to balance their position against price changes.  
- **Dynamic Hedging:** As the underlying price, time, and volatility change, dealers adjust their underlying positions to stay balanced based on gamma, vanna, and charm.  

### Dealer Gamma Positions

Dealers use gamma to manage their risk when trading options. Gamma affects how much dealers buy or sell the underlying as its price changes. There are two types of gamma positions:

- **Positive Gamma (Long Gamma):**  
  - **Effect on Market:** Tends to dampen big moves because the dealer’s hedging activity fights the direction of price changes.  
  - **Hedging Flows:**  
    - Price ↑ → Long-gamma dealer sells the underlying to stay delta‐neutral (which can push the price back down).
    - Price ↓ → Long-gamma dealer buys the underlying (which can push the price back up).

- **Negative Gamma (Short Gamma):**  
  - **Effect on Market:** Tends to exacerbate moves.  
  - **Hedging Flows:**  
    - Price ↑ → Short-gamma dealer buys (chasing the move higher). 
    - Price ↓ → Short-gamma dealer sells (pushing it lower).

### Dealer Vanna Positions

Vanna measures how an option's delta changes when implied volatility (IV) changes. When IV moves, dealers need to adjust their underlying hedge positions.

- **Positive Vanna (Long Vanna):**  
  - **Effect on Market:** When IV rises, positive vanna increases delta, requiring dealers to sell underlying to stay neutral. This can provide some resistance to upward moves during volatility spikes.
  - **Hedging Flows:**  
    - IV ↑ → Delta increases, so dealer sells underlying to rebalance (can dampen rallies).
    - IV ↓ → Delta decreases, so dealer buys underlying to rebalance (can support declines).

- **Negative Vanna (Short Vanna):**  
  - **Effect on Market:** When IV rises, negative vanna decreases delta, requiring dealers to buy underlying. This can amplify moves during volatility events.
  - **Hedging Flows:**  
    - IV ↑ → Delta decreases, so dealer buys underlying to rebalance (can fuel rallies).
    - IV ↓ → Delta increases, so dealer sells underlying to rebalance (can accelerate declines).

### Dealer Charm Positions

Charm measures how an option's delta changes as time passes (time decay). As options approach expiration, dealers must adjust their hedge positions due to changing delta.

- **Positive Charm (Long Charm):**  
  - **Effect on Market:** As time passes, positive charm typically decreases delta, requiring dealers to buy back underlying. This creates modest buying pressure over time.
  - **Hedging Flows:**  
    - Time passes → Delta decreases, so dealer reduces short hedge by buying underlying.
    - This creates gradual buying pressure, especially into close or over weekends.

- **Negative Charm (Short Charm):**  
  - **Effect on Market:** As time passes, negative charm typically increases delta, requiring dealers to sell more underlying. This creates modest selling pressure over time. 
  - **Hedging Flows:**  
    - Time passes → Delta increases, so dealer increases short hedge by selling underlying.
    - This creates gradual selling pressure, especially into close or over weekends.

### Standard Dealer Hedging Logic

Note: this is simplified. Hedge positions may be adjusted based on overall dealer exposure.  

| Investor Action  | Dealer Reaction  | Dealer Initial Hedge              | Position Closed or Expired     |
| ---------------- | ---------------- | --------------------------------- | ------------------------------ |
| Buy Call Option  | Sell Call Option | Buy Underlying (hedge short call) | Sell Underlying (remove hedge) |
| Buy Put Option   | Sell Put Option  | Sell Underlying (hedge short put) | Buy Underlying (remove hedge)  |
| Sell Call Option | Buy Call Option  | Sell Underlying (hedge long call) | Buy Underlying (remove hedge)  |
| Sell Put Option  | Buy Put Option   | Buy Underlying (hedge long put)   | Sell Underlying (remove hedge) |

---

## Economic Data Information

Review an economic calendar daily to identify news that may impact the market.  
Knowing that it's OPEX week may also matter, as institutions update positions and dealers unwind hedges. These flows can be very large.  

- [Why OPEX Matters](https://www.youtube.com/watch?v=tIf-XGfY5UM)  
- Economic Calendars:  
  - https://www.forexfactory.com/calendar  
  - https://us.econoday.com/byweek?cust=us  
  - https://www.marketwatch.com/economy-politics/calendar  
  - https://www.investing.com/economic-calendar/  
- [OPEX Calendar](https://www.marketwatch.com/tools/options-expiration-calendar)  
- [Fed Calendar](https://www.federalreserve.gov/newsevents/calendar.htm)  
- [FOMC Target Rate Probability](https://www.cmegroup.com/markets/interest-rates/cme-fedwatch-tool.html)  
- [Futures Equity Index Roll Dates](https://www.cmegroup.com/trading/equity-index/rolldates.html)  

---

## Tools

⚠️ Don’t subscribe to any “signals” services.  

### Options Dealer Exposure

Best tools to view options dealer exposures:  

- https://optionsdepth.com  
- https://vol.land  
- https://gexbot.com
- https://spotgamma.com (IMO pioneered GEX services to retail trader)

Free (delayed/naive):  
- https://gflows.app  
 

### Order Book

BookMap helps visualize the orderbook (useful for more liquid assets).  

- https://bookmap.com/en  
