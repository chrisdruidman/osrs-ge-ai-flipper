# OSRS Grand Exchange AI Flipper

🚀 **An intelligent Old School RuneScape market analysis tool that identifies profitable item flipping opportunities on the Grand Exchange.**

## 🎯 What This Tool Does

This application analyzes real-time OSRS market data to:

-   **Identify profitable flip opportunities** with buy/sell price recommendations
-   **Track your trade performance** and completion rates
-   **Provide market insights** using AI-powered analysis
-   **Monitor price trends** and volume patterns
-   **Calculate risk-adjusted profit potential**

## ✨ Key Features

### 🧠 AI-Powered Analysis

-   **Smart Price Prediction**: Machine learning models analyze market trends
-   **Risk Assessment**: Evaluate flip potential vs. market volatility
-   **Optimal Timing**: Identify the best windows for buy/sell orders
-   **Volume Validation**: Ensure sufficient liquidity for your trades

### 📊 Market Intelligence

-   **Real-time Price Data**: Live updates from OSRS Wiki API
-   **Historical Trends**: 30+ days of price history for pattern recognition
-   **Item Filtering**: Focus on high-volume, profitable items
-   **Market Sentiment**: Community-driven insights (future feature)

### 📈 Trade Management

-   **Flip Recommendations**: Curated list with buy/sell prices
-   **Performance Tracking**: Monitor your trade success rates
-   **Progress Updates**: Track partially filled orders
-   **Profit Analytics**: Detailed ROI and efficiency metrics

## 🛠️ Technology Stack

-   **Backend**: Node.js with Fastify (high performance, production-ready)
-   **Frontend**: React 18 with Vite and Tailwind CSS
-   **Database**: SQLite (simple, effective for market data)
-   **AI Integration**: Anthropic Claude 3.5 Sonnet + OpenAI GPT-4 fallback
-   **Authentication**: JWT with refresh tokens, bcrypt password hashing
-   **APIs**: OSRS Wiki Real-time API, RuneLite GE API (fallback)

## 🚀 Quick Start

### Prerequisites

-   Node.js 18+ (for both backend and frontend)
-   npm (package manager)
-   Anthropic API key (for Claude 3.5 Sonnet)
-   OpenAI API key (for GPT-4 fallback)

### Installation

1. **Clone the repository**

    ```bash
    git clone <repository-url>
    cd osrs-ge-ai-flipper
    ```

2. **Set up environment**

    ```bash
    cp .env.example .env
    # Edit .env with your configuration
    ```

3. **Install dependencies and start servers**

    ```bash
    # Install and start backend
    cd backend && npm install && npm run dev

    # In another terminal, install and start frontend
    cd frontend && npm install && npm run dev
    ```

4. **Access the application**
    - Frontend: http://localhost:5173
    - Backend API: http://localhost:3000
    - API Documentation: Available via backend endpoints

## 📖 How to Use

### 1. Get Flip Recommendations

-   Navigate to the Dashboard
-   Review AI-generated flip opportunities
-   Filter by profit potential, volume, or risk level
-   Note the recommended buy/sell prices

### 2. Execute Trades In-Game

-   Use the recommended prices as starting points
-   Place buy orders slightly above recommended buy price
-   Place sell orders at or near recommended sell price
-   Adjust based on current market conditions

### 3. Track Performance

-   Input your actual trade details
-   Update trade status (bought, sold, partial)
-   Monitor completion rates and profitability
-   Analyze your trading patterns

## 🎮 OSRS Trading Tips

### Understanding the Grand Exchange

-   **Buy Limits**: Each item has a 4-hour purchase limit
-   **Offer Duration**: Orders expire after a certain time
-   **Market Fluctuations**: Prices change based on supply/demand
-   **Instant vs. Patient**: Balance speed vs. profit margins

### Best Practices

-   Start with small volumes to test strategies
-   Diversify across multiple items
-   Monitor trade completion rates
-   Adjust strategies based on performance data
-   Consider peak playing hours for volume

## 🔄 Development Status

This project is currently in active development. See `HANDOVER_SUMMARY.md` for the latest progress and next steps.

### Current Phase: Foundation Setup ✅

-   [x] Project structure and guidelines
-   [x] Technology stack decisions
-   [x] Documentation framework
-   [x] Development workflow

### Next Phase: Backend Infrastructure

-   [ ] FastAPI application setup
-   [ ] Database schema and models
-   [ ] OSRS API integration
-   [ ] Basic flip detection algorithm

## 🤝 Contributing

This project uses an agent-based development approach. Each development phase is handled by specialized agents following the guidelines in `.cursor/rules`.

### For Developers

1. Review `.cursor/rules` for coding standards and guidelines
2. Check `HANDOVER_SUMMARY.md` for current status
3. Follow the established project structure
4. Update handover documentation when completing phases

### For OSRS Players

-   Report bugs or suggest features via issues
-   Share trading strategies and market insights
-   Provide feedback on flip recommendations
-   Help test new features

## 📊 Data Sources

-   **Primary**: [OSRS Wiki Real-time API](https://prices.runescape.wiki/api/v1/osrs/)
-   **Fallback**: RuneLite Grand Exchange API
-   **Item Database**: OSRS Wiki item mappings
-   **Historical Data**: 5-minute interval price history

## ⚖️ Legal & Ethics

-   **No Account Access**: This tool never requires your OSRS login
-   **Read-Only APIs**: Only uses publicly available market data
-   **Player Responsibility**: All trading decisions and actions are yours
-   **Risk Disclosure**: Flipping involves financial risk in-game
-   **Fair Play**: Complies with OSRS rules and Jagex terms of service

## 📄 License

This project is open source. See LICENSE file for details.

## 🆘 Support

-   **Documentation**: Check the `docs/` directory
-   **API Issues**: Verify OSRS Wiki API status
-   **Development Help**: Review `.cursor/rules` and handover docs
-   **OSRS Questions**: Consult the [OSRS Wiki](https://oldschool.runescape.wiki/)

---

**Disclaimer**: This tool is for educational and entertainment purposes. Trading on the Grand Exchange involves in-game financial risk. Always do your own research and trade responsibly.
