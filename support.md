---
layout: default
title: Support
---

# Support

## Frequently Asked Questions

### Getting Started

**How do I add a session?**

Tap the + button on the Home tab. You can use "Quick Add" for fast entry or "Full Session" for more details.

**How do I end an active session?**

Tap on the active session from the Home screen, then tap "End Session" and enter your final amount.

**What's the difference between Quick Add and Full Session?**

- **Quick Add**: Streamlined entry for starting a session quickly with just the buy-in amount
- **Full Session**: Complete form for entering all details including location, category, trip, and notes

### Data & Sync

**Is my data backed up?**

If you have iCloud enabled, your data automatically syncs across all your devices signed into the same Apple ID.

**How do I export my data?**

Go to the Sessions tab, tap the export button (share icon), and choose where to save your CSV file.

**How do I delete all my data?**

You can delete individual sessions by swiping left on them in the Sessions list. To delete all data, you can delete and reinstall the app.

### Categories & Locations

**How do I add a new category?**

Tap the menu icon (hamburger menu) and select "Manage Categories", then tap the + button.

### Trips

**What are trips for?**

Trips help you group sessions together, such as a weekend in Vegas or a cruise. You can view profit/loss summaries by trip.


### Charts & Summary (Included with Base App)

The Profit Over Time chart on the Summary screen is available to all users at no cost.

**How does the Profit Over Time chart work with time filters?**

The **Profit Over Time** chart on both the Home and Summary screens shows your cumulative profit/loss over time.

When a **time filter** is applied (e.g. "2026", "This Month"), the chart carries over your cumulative total from all prior periods as a **baseline starting point**. This means the chart line starts at your ending position from the previous period, so you can see your absolute cumulative position while focusing on the selected time range.

**Example:**
- Your cumulative profit through end of 2025: $22,000
- You filter to "2026"
- The chart starts at $22,000 and plots 2026 sessions from there

The **summary numbers** (Sessions, Net Total) above the chart show only the profit/loss earned **within the selected period**, not including the baseline.

**What does the "Change" percentage mean on the Summary screen?**

The **Change** percentage shows the **percentage change relative to your starting baseline** for the selected time period.

**Formula:**
```
Change = (Period Profit/Loss ÷ Baseline Cumulative Profit) × 100
```

**Example:**
- Your cumulative profit entering 2026: $22,000 (baseline)
- Your 2026 profit so far: $1,366
- Change = $1,366 ÷ $22,000 × 100 = **+6.2%**

**Notes:**
- A positive percentage (green) means you grew your bankroll during this period
- A negative percentage (red) means you lost ground during this period
- For **All Time**, the baseline is 0 and Change shows **0%** since there is no prior period to compare against

---

## Premium Features

Premium subscribers get access to advanced analytics charts on the Insights screen. Swipe between charts to explore different views of your data. All charts below require a Premium subscription.

### Win/Loss Rate by Category

A donut chart showing win or loss rate for each category. Swipe left/right to toggle between Win Rate and Loss Rate views.

**How to read the chart:**

The chart displays **two dimensions** of information:
- **Slice size** = Number of sessions (how much you play this category)
- **Percentage label** = Win/loss rate (how often you win or lose)

This design helps you spot patterns:
- **Large slice + low win rate** = Problem area (you play it often but lose frequently)
- **Small slice + high win rate** = Opportunity (you're good at it but don't play much)
- **Large slice + high win rate** = Your strength (keep doing what works!)

**Win Rate Formula:**
```
Win Rate = (Sessions with Profit > $0 ÷ Total Sessions) × 100
```

**Loss Rate Formula:**
```
Loss Rate = (Sessions with Profit < $0 ÷ Total Sessions) × 100
```

**Example:**
- You have 50 Blackjack sessions
- 30 ended with profit > $0, 15 ended with loss < $0, 5 broke even
- Win Rate = 30 ÷ 50 × 100 = **60%**
- Loss Rate = 15 ÷ 50 × 100 = **30%**

**Notes:**
- A "win" is any session ending in profit, regardless of amount
- Win Rate + Loss Rate may not equal 100% if you have break-even sessions
- Categories can be excluded from these charts in category settings (Premium)
- Sessions without a category appear as "Uncategorized"
- Top 3 categories are shown individually; remaining categories are grouped into "Other Categories"

### Profit by Location

A bar chart showing your total profit or loss at each casino/location. Helps identify which venues are most profitable for you.

### Best Playing Times

A heatmap grid showing your average profit/loss by day of the week and time of day. Each cell is colored from red (worst) through gray (break-even) to green (best), with the number inside showing how many sessions fall in that slot.

**Time blocks:**
- **Morning** — 6:00 AM to 11:59 AM
- **Afternoon** — 12:00 PM to 4:59 PM
- **Evening** — 5:00 PM to 9:59 PM
- **Late Night** — 10:00 PM to 5:59 AM

**How to read the chart:**
- **Color** = Average profit/loss for that day and time slot (green is profitable, red is unprofitable)
- **Number** = How many sessions you played in that slot
- **Gradient bar** = Shows the full color scale with dollar amounts for the current data range

Tap any cell to see the individual sessions behind it.

**Notes:**
- Sessions are bucketed by their start time
- The color scale is relative to your data — the brightest green is your best slot, the brightest red is your worst
- Empty cells (no sessions) appear as dark gray
- Respects the active time filter (This Year, Last Month, etc.)

### Bankroll Health

A summary card at the top of the Insights screen showing an overall health label based on three normalized factors. Tap the card to drill down into the raw metrics behind each factor.

**Factor 1: Net Trend (Direction)**
Are you generally up or down over time? Combines session profit/loss with comps and expenses.

- Uses a sigmoid curve to map net P/L to a 0–100 score (50 = breakeven, scales smoothly in both directions)
- **↑ Positive** (green, score ≥ 60) — Bankroll is growing
- **→ Flat** (orange, score 40–59) — Bankroll is holding steady
- **↓ Negative** (red, score < 40) — Losses are outpacing gains

**Factor 2: Volatility per Hour (Stability)**
How wild are your swings relative to time played? Measures average |profit or loss| per session hour.

- Sessions under 5 minutes are excluded to avoid extreme outliers
- Lower volatility = higher score (more sustainable bankroll health)
- **Low** (green, score ≥ 60) — Steady, predictable sessions
- **Moderate** (orange, score 30–59) — Notable swings per hour
- **High** (red, score < 30) — Large swings relative to time played

**Factor 3: Comp Offset Ratio (Buffer)**
How much do comps and income soften your losses?

**Formula:**
```
Comp Offset = Total Income ÷ Gross Session Losses × 100
```

- **30%+** (green) — Strong cushion. Comps significantly soften losses.
- **10–29%** (orange) — Meaningful buffer. Comps help but don't fully cover losses.
- **<10%** (red) — Minimal buffer. Comps barely dent losses.
- **No losses** (green) — No session losses to offset.

**Overall Score:**
Each factor is normalized to 0–100, then averaged:

```
Bankroll Health Score = (Net Trend + Volatility + Comp Offset) ÷ 3
```

| Score | Label | Color |
|-------|-------|-------|
| 80–100 | Strong | Green |
| 60–79 | Stable | Blue |
| 40–59 | At Risk | Orange |
| < 40 | Unstable | Red |

**Drill-Down Detail:**
Tap the card to see the raw numbers behind each factor:
- Net Trend: session P/L, transaction P/L, combined net, factor score
- Volatility: average $/hr swing, sessions analyzed, total hours, factor score
- Comp Offset: total comps, gross losses, offset ratio, factor score

**Notes:**
- Respects the active time filter (This Year, Last Month, etc.), or uses all data when no filter is selected
- "Gross losses" counts only sessions that ended with negative profit (not net losses)
- Income includes all income-category transactions (comps, freeplay, etc.)
- Volatility uses absolute value of P/L — a $200/hr win and $200/hr loss are equally volatile

### Stability Factors

A companion card to Bankroll Health that focuses on behavioral patterns and risk concentration. Tap to drill down into detailed metrics for each factor.

Each row shows a factor name, a status icon (✅ green = healthy, ⚠️ orange = needs attention), and the current value. Here's what each factor measures:

**Session Volatility**
Reuses the volatility score from Bankroll Health (average |win or loss| per session hour).
- ✅ **Low** — score ≥ 60 (avg swing under ~$80/hr)
- ⚠️ **Moderate/High** — score < 60

**Loss Recovery Rate**
How often a losing session is followed by a winning session. Measures discipline and tilt resistance.

- Sessions are sorted chronologically; each loss with a following session is an "opportunity"
- If the next session is a win (P/L > 0), it counts as a "recovery"
- Breakeven sessions (P/L = 0) count as neither a loss nor a recovery
- ✅ **Healthy** — recovery rate ≥ 50%
- ⚠️ **Low** — recovery rate < 50%
- Display format: `recoveries/opportunities (rate%)`

**Comp Offset**
Reuses the comp offset score from Bankroll Health.
- ✅ **Strong** — score ≥ 60 (offset ratio ≥ 18%)
- ⚠️ **Moderate/Minimal** — score < 60

**Biggest Loss Ratio**
Your largest single session loss as a percentage of total money committed (sum of all startMoney).

**Formula:**
```
Biggest Loss Ratio = Largest Single |Loss| ÷ Sum of All startMoney × 100
```

- ✅ **Healthy** — ratio ≤ 20%
- ⚠️ **Elevated** — ratio > 20% (one bad session had outsized impact)
- Display format: `$amount (ratio%)`

**Drill-Down Detail:**
Tap the card to see the raw numbers behind each factor:
- Session Volatility: avg swing/hr, sessions analyzed, total hours, volatility score
- Loss Recovery: wins after losses, total loss opportunities, recovery rate
- Comp Offset: total comps, gross losses, offset ratio, comp score
- Biggest Loss Ratio: largest single loss, total money committed, concentration ratio

**Notes:**
- Respects the active time filter
- Shares volatility and comp offset calculations with the Bankroll Health card
- Loss recovery requires at least 2 completed sessions to produce meaningful data

### Duration vs Profit

A scatter plot showing the relationship between session duration and profit/loss. Helps identify if longer sessions tend to be more or less profitable.

---

## Troubleshooting

**The app won't open**

Try force-quitting and restarting the app. If the problem persists, restart your device.

**My data isn't syncing**

1. Ensure you're signed into iCloud
2. Check that iCloud is enabled for SessionTracker in Settings > [Your Name] > iCloud
3. Ensure you have an internet connection

**Charts aren't showing any data**

Charts only display completed sessions. Make sure you have ended some sessions with final amounts.

## Contact Us

If you need further assistance or want to report a bug, please fill out our support form:

**[Contact Support](https://forms.gle/3eshCUtCe4daA9Nc7)**

We typically respond within 24-48 hours.

## Responsible Gaming Resources

If you or someone you know needs help with problem gambling:

- **National Council on Problem Gambling**: 1-800-522-4700
- **Gamblers Anonymous**: [www.gamblersanonymous.org](https://www.gamblersanonymous.org)
- **National Problem Gambling Helpline**: Available 24/7

---

[Back to Home](/)
