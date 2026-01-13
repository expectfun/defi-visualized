# defi-visualized

Interactive visualizations that explain DeFi concepts. Each example is a single HTML file with no dependencies — just open in a browser and explore.

## Goal

DeFi concepts often involve mathematical relationships that are hard to grasp from text alone. These interactive tools let you adjust parameters and immediately see the effects, building intuition for how these systems actually work.

## Examples

### Bonding Curve
**File:** `bonding-curve.html`

Explore how token price changes based on supply. Visualizes the core mechanic behind many token launches and AMMs.

**Features:**
- Multiple curve types: Linear, Quadratic, Cubic, Square Root, Exponential
- Adjustable steepness parameter
- Buy/Sell simulation with +/- 10 token buttons
- Total reserve visualization (area under curve)
- Live stats: current price, market cap, next token cost

**Concepts demonstrated:**
- Price discovery through mathematical functions
- Why early buyers get better prices
- How reserve (collateral) accumulates
- The relationship between curve shape and price dynamics

---

## Ideas for Future Visualizations

### AMM Price Impact (x × y = k)
Visualize the constant product formula used by Uniswap and similar DEXs.
- Show the xy=k curve with current pool state
- Simulate swaps of different sizes
- Demonstrate slippage: small trades vs large trades
- Show how liquidity depth affects price impact

### Impermanent Loss
The hidden cost of providing liquidity that confuses many newcomers.
- Plot IL percentage against price divergence
- Slider to adjust "price changed by X%"
- Compare: LP position value vs just holding
- Show why it's "impermanent" (recovers if price returns)

### Liquidation Threshold
Visualize the danger zone in collateralized lending.
- Health factor gauge that responds to price changes
- Adjust collateral amount, debt amount, asset price
- Show liquidation penalty impact
- Compare different collateral ratios

### APY vs APR Compounding
Demystify the difference between APR and APY.
- Same nominal rate, different compounding frequencies
- Time slider shows growth curves diverging over time
- Calculator: "What does 100% APR actually yield?"
- Compare daily, weekly, monthly, yearly compounding

### Token Vesting Schedules
Understand how token unlocks work.
- Compare cliff vs linear vs custom schedules
- Timeline showing unlocked vs locked tokens
- Multiple vesting schedules overlaid
- Calculate "fully diluted" vs "circulating" supply

### Vote-Escrow (veToken) Decay
Visualize the mechanics behind Curve's ve model.
- Lock duration slider (1 week to 4 years)
- Show voting power over time as lock decays
- Demonstrate the tradeoff: longer lock = more power
- Compare different lock strategies

### Leverage & Liquidation Price
Understand the risks of leveraged trading.
- Adjust leverage from 1x to 100x
- See liquidation price move closer to entry
- Visualize profit/loss curves at different leverage
- Show how fees and funding affect the position

### Dutch Auction
Price discovery through descending price auctions.
- Price decreasing over time curve
- Simulate different bidder entry points
- Show clearing price mechanics
- Used in NFT mints and token launches

---

## Design Principles

1. **Single file**: Each example is one self-contained HTML file
2. **No dependencies**: Works offline, no build step, no npm
3. **Mobile-friendly**: Responsive layout that works on any screen
4. **Immediate feedback**: Every input change updates the visualization instantly
5. **Show the math**: Display formulas so users connect visuals to equations

---

## Contributing

Ideas for new visualizations welcome. Each should:
- Explain one core DeFi concept
- Be interactive (not just static diagrams)
- Build intuition through exploration
- Include the actual formulas/math involved
