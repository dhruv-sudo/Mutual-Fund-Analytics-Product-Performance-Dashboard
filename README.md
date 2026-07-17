# Mutual-Fund-Analytics-Product-Performance-Dashboard
Interactive Power BI dashboard for analyzing mutual fund performance, risk metrics, AUM, NAV trends, and investment insights using SQL, Python, Excel, and DAX.
This GitHub Pages URL previously hosted the live app. It's now retired — the app lives on a new, privately-hosted home:

🔗 my-mf-dashboard.pages.dev

If you used the app at this address before, visit the page above — it has a one-click Export My Data option to back up your locally-saved goals, preferences, and cached portfolio data, so you can restore everything on the new site in under a minute...

The source code for this project is now maintained privately.

✨ Features
📈 Portfolio Insights
Real-time Portfolio Tracking: Monitor current value, gains/losses, and returns
Asset Allocation: Visualize distribution across equity, debt, gold, and silver
Market Cap Analysis: Track large-cap, mid-cap, and small-cap exposure
Sector Distribution: Understand your equity sector allocation
Fund House Distribution: See your AMC-wise portfolio split
Holdings Analysis: Deep dive into individual stock holdings across funds
💰 Performance Metrics
XIRR Calculation: Accurate returns using Extended Internal Rate of Return
Absolute Returns: Track overall and individual fund performance
Realized vs Unrealized Gains: Separate tracking of booked and paper profits
Weighted Portfolio Returns: 1Y, 3Y, and 5Y weighted returns across all holdings
Benchmark Comparison: Portfolio vs Nifty 50 and Nifty 500
Alpha Analysis: Outperformance and underperformance across 1Y, 3Y, and 5Y periods
Visual Return Comparison: Side-by-side benchmark comparison charts
Fund-Level XIRR: Individual XIRR calculation for each fund
📊 Visual Analytics
Interactive Charts: Chart.js visualizations for all metrics
Growth Tracking: Monitor portfolio value over time with daily valuation
Investment Flow: Track monthly/quarterly/yearly investments and redemptions
Fund Valuation History: Individual fund performance charts
Performance Comparison: Compare fund vs category vs benchmark returns
Performance vs Benchmark Chart: All holdings indexed to 100 at period start — compare any combination of funds against Nifty 50 and Nifty 500 over 1Y, 2Y, 3Y, 5Y, 7Y, or 10Y periods. Partial-history funds shown with a "since MMM 'YY" label.
Portfolio Allocation Chart: Horizontal bar chart showing each fund's share of the total current portfolio value at a glance
💸 Capital Gains
Tax Calculation: Automatic STCG and LTCG calculation with proper categorization
Financial Year Reports: Year-wise capital gains breakdown (FY 2019-20 onwards)
Transaction-Level Details: FIFO-based cost basis tracking
Downloadable Reports: Export capital gains as Excel files (FY-wise or all-time)
Current Year Tracking: Real-time tracking of current financial year gains
📝 Transaction Management
Complete Transaction History: All purchases, redemptions, and switches
Two Views: All-time transactions or active holdings only
Folio-wise Tracking: Separate tracking for multiple folios
Excel Export: Download transaction reports in XLSX format
Real-time NAV Updates: Fetch latest NAV data automatically
📅 Portfolio Analysis & Projection
Portfolio History Charts: Interactive growth, investment, withdrawal, and net investment views with time filters (1M to All)
Average Monthly Summary: Average buy/sell/net inflow over the last 6M and 12M
Portfolio Projection: SIP-style future value calculator with configurable CAGR, annual step-up %, and custom SIP amount — projected up to 20 years
Transaction Calendar: Visual heatmap showing days you invested (green) or withdrew (red), browsable by year (2019–2026)
🔒 Data Management
Local Storage: All data stored in browser's IndexedDB — never leaves your device
No Server Storage: Financial data is processed transiently and deleted immediately after parsing
Auto-Updates: Intelligent daily NAV and monthly stats updates
Cache Control: Manual cache refresh and clear options
Duplicate Prevention: Smart detection of already-uploaded CAS files
🔄 Auto-Update Features
The application automatically keeps your portfolio data fresh:

4x-Daily NAV Updates ⏰

Automatically fetched at 12 AM, 9 AM, 9:30 PM, 12 PM IST each day
Each slot triggers a refresh if the last NAV update predates that slot
Incremental — only new data is fetched and merged
Runs silently in the background
No separate manual NAV trigger — use Update Stats to force an immediate full refresh (resets both the NAV and 7-day stats clock)
Weekly Fund Statistics Updates 📅

Triggered automatically every week
Fetches portfolio composition, returns, ratings, holdings, and expense ratios
Manual trigger available from the Manage Data tab
Limited to once per week
Non-blocking background process
Weekly Benchmark Data Updates 📊

Fetches Nifty 50 TRI and Nifty 500 TRI trailing returns (1Y/3Y/5Y/10Y) and rolling return averages
Stored globally in browser localStorage (shared across all users)
Refreshed automatically once per week in the background
Powers the Performance vs Benchmark table and portfolio alpha calculations
Smart Update Tracking: The Manage Data tab shows last-updated timestamps for CAS parsing, fund stats, and NAV.

🔍 Advanced Analysis Tools
Overlap Analysis: Identify duplicate holdings across funds

Pairwise fund overlap with percentage and common stock count
Stocks held across multiple funds with average weight
Helps eliminate redundancy and reduce concentration risk
Expense Impact Analysis: Understand the true cost of fund management

Weighted expense ratio across the portfolio
Annual and lifetime cost projections per fund
Highlights high-cost funds for optimization
Portfolio Health Score: Data-driven quality assessment (0–100, A+ to D)

Diversification score (25 pts) — fund count
Expense Ratio score (25 pts) — weighted ER
Performance score (25 pts) — funds beating benchmark
Overlap score (25 pts) — high/medium overlap pairs
Actionable improvement suggestions per dimension
🏦 Tax Planning
Long-Term vs Short-Term Split: Holdings value and unrealized gain by holding period
Unrealized LTCG & STCG: Know your tax exposure before you redeem
Tax Optimization Tips: LTCG harvesting up to the ₹1.25L annual exemption, hold-period strategy, rebalancing timing
👨‍👩‍👧‍👦 Multi-User & Family Dashboard
Multiple Portfolios: Track portfolios for your entire family
User Management: Add, switch, and delete users from the Manage Data tab
Separate Storage: Each user's data stored independently
Family Dashboard: Aggregated view across all users (visible when 2+ users exist)
Combined family value, cost, P&L, and unique holdings count
Family-wide asset allocation, fund house distribution, and sector breakdown
Equity market cap split across all portfolios
Family weighted returns (1Y, 3Y, 5Y)
Family benchmark comparison against Nifty 50 and Nifty 500
Family alpha generation metrics
Family performance visualization
Per-member breakdown with value, cost, P&L, and active holdings count
📱 Progressive Web App (PWA)
Installable: Add to home screen on mobile or desktop
Offline Ready: Works without internet after initial load
App-like Experience: Full-screen mode, native feel
Auto Updates: Service worker manages updates seamlessly
📷 Screenshot Export
Full dashboard screenshot capture
Desktop and mobile screenshot buttons
Share portfolio snapshots instantly
