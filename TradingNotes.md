## Day Trading Opinionated

These are the main tools and ideas that I use in my trading.

### Understanding Market Structure

**Key Price Levels:** Identify important prices where the market often changes direction.

**Understanding Market Structure for Trading:** https://youtu.be/sgAnVR6RSDg?si=Z8zKjSa3pxBMW84U

### Footprint Charts

**Delta:** Shows whether there's more buying or selling.

**Imbalances:** Highlights when buyers or sellers are overpowering the market.

**Absorption:** Indicates large orders being absorbed at certain prices.

**Exhaustion:** Signals slowing activity, which might mean a trend is about to change.

**Understanding Footprint Charts:** https://www.youtube.com/watch?v=6lRy3QdLciM

### Volume Profile

**Market Depth Insight:**  Understand where the majority of trading activity occurs at specific price levels.

**Key Levels:** Identify high-volume nodes (areas of significant interest) and low-volume nodes (potential support/resistance zones).

**Volume Profile Trading:** https://www.youtube.com/watch?v=vVMJa7dyYWE

### Options and Their Influence on the Underlying

Even if you don’t trade options, it's important to know that options can influence the underlying price. Understanding this helps you possibly anticipate price movements based on how much options market makers (dealers) are exposed to. Even though this is a high-level overview, these topics are more advanced and you don't need to know them in detail. You just need to basically understand that it can impact the market because the dealer may suppress or amplify the moves based on the dealer exposure.

**How Options Moves the Markets:** https://youtu.be/0oJqC9QK-I0?si=YM_tOxYeLYYIEnuY

**Understanding GEX:** https://www.youtube.com/watch?v=xWLx3vPfe7U

**Understanding VEX:** https://www.youtube.com/watch?v=PUlVpSJJdfw

**Understanding CEX:** https://www.youtube.com/watch?v=lUXhZ1asBRQ

#### Key Terms

**Gamma:** Measures how quickly an option’s sensitivity (delta) changes as the underlying price moves. High gamma means delta changes rapidly.

**Vanna:** Measures how an option’s delta changes when the underlying volatility changes. High vanna means delta is very sensitive to volatility.

**Charm:** Measures how an option’s delta changes over time, often decreasing as the option gets closer to expiration.

#### Hedging Options

**Initial Delta Hedge:** When dealers trade options, they buy or sell the underlying to balance their position against price changes.

**Dynamic Hedging:** As the underlying price, time, and volatility change, dealers adjust their underlying positions to stay balanced based on gamma, vanna, and charm.

#### Dealer Gamma Positions

Dealers use gamma to manage their risk when trading options. Gamma affects how much dealers buy or sell the underlying as its price changes. There are two types of gamma positions.

**Positive Gamma (Long Gamma):**

**Effect on Market:** Tends to dampen big moves because the dealer’s hedging activity fights the direction of price changes.

**Hedging Flows:**

- When the underlying rises, a long‐gamma dealer sells the underlying to stay delta‐neutral (which can push the price back down).
- When the underlying falls, a long‐gamma dealer buys the underlying (which can push the price back up).

**Negative Gamma (Short Gamma):**

**Effect on Market:** Tends to exacerbate moves.

**Hedging Flows:**

- When the underlying rises, a short‐gamma dealer buys (chasing the move higher).
- When the underlying falls, a short‐gamma dealer sells (pushing it lower).

#### Dealer Vanna Positions

Vanna affects how dealers respond to changes in implied volatility, causing them to buy or sell the underlying as IV shifts.

**Positive Vanna (Long Vanna):**

**Effect on Market:** If implied volatility increases, a long‐vanna position often leads dealers to adjust their hedge in ways that partially counter the price move.

**Hedging Flows:**

- When implied volatility rises, a positive‐vanna dealer’s delta may increase, prompting the dealer to sell some of the underlying to stay delta‐neutral.
- When implied volatility falls, a positive‐vanna dealer’s delta may decrease, leading them to buy the underlying to rebalance.

**Negative Vanna (Short Vanna):**

**Effect on Market:** Large swings in IV can increase volatility in the underlying because dealers are forced to chase the move with their hedges.

**Hedging Flows:**

- When implied volatility rises, a short‐vanna dealer’s delta may decrease, leading them to buy the underlying (chasing the move higher).
- When implied volatility falls, a short‐vanna dealer’s delta may increase, causing them to sell the underlying (further pressuring it lower).

#### Dealer Charm Positions

Charm captures how dealers must adjust their hedge as time to expiration changes delta.

**Positive Charm (Long Charm):**

**Effect on Market:** Can smooth price action intraday or over short periods because dealers steadily adjust their hedges as delta decays.

**Hedging Flows:**

- As time passes and delta decays, a long‐charm dealer’s net delta often decreases more slowly. They may buy back some of the underlying over time to maintain a neutral position.
- If the option is moving deeper in‐the‐money (increasing delta) as time passes, the charm effect can lead to a gradual selling of the underlying to stay hedged.

**Negative Charm (Short Charm):**

**Effect on Market:** Can contribute to intraday or overnight volatility as dealers must make larger, more reactive hedges.

**Hedging Flows:**

- As time passes, a short‐charm dealer’s net delta may shift faster, forcing them to sell or buy the underlying more aggressively.
- This can accelerate price moves if a large short‐charm position needs continuous rebalancing.

#### Standard Dealer Hedging Logic

Note that this is simple table and hedge positions could be partially removed due to other positions dealers may still need to hedge.

| Investor Action  | Dealer Reaction  | Dealer Initial Hedge              | Position Closed or Expired     |
| ---------------- | ---------------- | --------------------------------- | ------------------------------ |
| Buy Call Option  | Sell Call Option | Buy Underlying (hedge short call) | Sell Underlying (remove hedge) |
| Buy Put Option   | Sell Put Option  | Sell Underlying (hedge short put) | Buy Underlying (remove hedge)  |
| Sell Call Option | Buy Call Option  | Sell Underlying (hedge long call) | Buy Underlying (remove hedge)  |
| Sell Put Option  | Buy Put Option   | Buy Underlying (hedge long put)   | Sell Underlying (remove hedge) |

## Economic Data Information

Make sure to review an economic calendar every day to identify potential news that may impact the market. In addition, knowing that its OPEX week may also affect the market as institutions update their positions and dealers start to unwind hedges. These options can be very large. Note the `How Options Moves the Markets` video above.

**Why OPEX Matters:** https://www.youtube.com/watch?v=tIf-XGfY5UM

**Economic Calendars:** https://www.forexfactory.com/calendar | https://us.econoday.com/byweek?cust=us | https://www.marketwatch.com/economy-politics/calendar | https://www.investing.com/economic-calendar/

**OPEX Calendar:** https://www.marketwatch.com/tools/options-expiration-calendar

**Fed Calendar:** https://www.federalreserve.gov/newsevents/calendar.htm

**FOMC Target Rate Probability:** https://www.cmegroup.com/markets/interest-rates/cme-fedwatch-tool.html

**Futures Equity Index Roll Dates:** https://www.cmegroup.com/trading/equity-index/rolldates.html

## Tools

DON'T subscribe to any "signals" services.

#### Options Dealer Exposure

The below are probably the best tools if you want to view the options dealer's exposures based on the data and how the calculate the exposures.

- https://optionsdepth.com
- https://vol.land
- https://gexbot.com

Free
- https://gflows.app (Free, Delayed, Naive)
- Bear Trap Discord https://discord.com/invite/beartrap

#### OrderBook

BookMap helps visualize the orderbook. I think this can be helpful for more liquid assets.

- https://bookmap.com/en
