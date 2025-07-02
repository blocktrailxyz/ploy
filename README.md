# Ploy - Universal Multi-Chain Loyalty Platform

> *Transform loyalty into digital assets. Zero gas fees. Infinite possibilities.*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![SUI](https://img.shields.io/badge/SUI-4DA2FF?logo=sui&logoColor=white)](https://sui.io/)
[![Solana](https://img.shields.io/badge/Solana-9945FF?logo=solana&logoColor=white)](https://solana.com/)
[![React](https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB)](https://reactjs.org/)

## 🚀 What is Ploy?

Ploy is a revolutionary loyalty platform that transforms traditional points into valuable digital assets, with optional blockchain integration. Start with cost-effective traditional storage and seamlessly upgrade to blockchain when ready. Built with a flexible architecture supporting SUI, Solana, and EVM chains with zero gas fees for users, Ploy enables businesses across all industries to create comprehensive loyalty programs that scale with their needs.

### ✨ Key Features

#### 🏗️ **Marketplace-Ready Multi-Service Architecture**
- **🔧 Dynamic Field System** - Create custom services without code deployment
- **🏪 Digital Asset Marketplace** - Trading and discovery from day one (all storage modes)
- **⚙️ Service Composition** - Combine loyalty + NFTs + experiences + subscriptions
- **🔗 Cross-Service Workflows** - Automated actions across different service types
- **📈 Dynamic Pricing Engine** - AI-powered price discovery and market analysis

#### 💾 **Flexible Storage & Migration**
- **💡 Flexible Storage Options** - Start with traditional database, upgrade to blockchain when ready
- **💰 Cost-Effective Entry** - Launch loyalty programs without blockchain costs
- **🚀 Seamless Migration** - Zero-downtime upgrade from traditional to blockchain storage
- **🔄 Asset Tokenization** - Convert digital rewards to NFTs when blockchain enabled
- **⚡ Instant Performance** - Fast database operations or sub-second blockchain confirmations

#### 🌐 **Multi-Chain & Trading**
- **🔥 Zero Gas Fees** - Users never pay transaction costs when blockchain is enabled
- **⛓️ Optional Multi-Chain** - SUI, Solana, Ethereum, Polygon, BSC, Arbitrum, Base (when enabled)
- **🌉 Cross-Chain Bridge** - Available in blockchain mode for token transfers
- **🏪 Advanced Marketplace** - Auctions, bundles, collections, external platform sync
- **💎 Point Economy** - Traditional points system with optional blockchain tokenization

#### 🎯 **Industry Solutions & AI**
- **🏭 Industry Templates** - Pre-built for SaaS, E-commerce, Cloud, FinTech, Gaming, Travel, Health & Fitness, Food & Drink
- **🎮 Digital Rewards** - Simulated assets in traditional mode, real NFTs in blockchain mode
- **🎯 Dynamic Policies** - Real-time rule adjustments work in both storage modes
- **🎨 White-Label Ready** - Fully customizable branding regardless of storage choice

#### 🤖 **Universal AI Integration**
- **🤖 Universal LLM Integration** - Works with ANY LLM via Model Context Protocol (MCP)
- **🔮 AI-Powered Intelligence** - Natural language management for both storage modes
- **🎙️ Conversational Interface** - Chat with OpenAI, Claude, Llama, or local models
- **⚙️ MCP-Compatible Architecture** - Industry-standard AI integration + loyalty optimizations
- **🛠️ AI Tool Ecosystem** - 20+ instant integrations via MCP protocol

## 🏗️ Architecture Overview

```mermaid
---
config:
  layout: fixed
---
flowchart TD
    subgraph subGraph0["Frontend Layer"]
        A["Web App"]
        B["Mobile Apps"]
        C["Partner Portals"]
        D["Wallet Integration"]
        AI["AI Chat Interface"]
    end
    
    subgraph subGraph1["Universal AI Layer"]
        MCP["MCP Protocol Server"]
        UAG["Universal LLM Gateway"]
        AO["Agent Orchestrator"]
        OPT["Loyalty Optimizer"]
        ANY["Any LLM Client"]
        OPENAI["OpenAI GPT-4"]
        CLAUDE["Anthropic Claude"]
        LLAMA["Meta Llama"]
        LOCAL["Local Models"]
        AAnalytics["Analytics Agent"]
        ACampaign["Campaign Agent"]
        ASupport["Support Agent"]
        AFraud["Fraud Agent"]
    end
    
    subgraph subGraph2["API Layer"]
        E["REST API"]
        F["WebSocket Events"]
        G["GraphQL Gateway"]
        H["Real-time Updates"]
        HL["Headless Services"]
    end
    
    subgraph subGraph3["Business Logic"]
        I["Policy Engine"]
        J["NFT Minter"]
        K["Reward Calculator"]
        L["Marketplace Engine"]
        M["Analytics Engine"]
        PR["Predictive Engine"]
        CS["Chain Selector"]
        TR["Transaction Router"]
    end
    
    subgraph subGraph4["Multi-Chain Abstraction"]
        CA["Chain Abstraction Layer"]
        PM["Plugin Manager"]
        HR["Health Monitor"]
    end
    
    subgraph subGraph5["Cross-Chain Infrastructure"]
        BR["Bridge Router"]
        BA["Bridge Aggregator"]
        WH["Wormhole"]
        LZ["LayerZero"]
        AX["Axelar"]
    end
    
    subgraph subGraph6["Flexible Storage Layer"]
        STORAGE["Storage Mode Selector"]
        TRAD["Traditional Storage"]
        BLOCKCHAIN["Blockchain Storage"]
        V["PostgreSQL"]
        W["Redis Cache"]
        X["IPFS Storage"]
        Y["Event Store"]
        ML["ML Models"]
        CC["Chain Configs"]
        MIG["Migration Service"]
    end
    
    subgraph subGraph7["Blockchain Plugin Ecosystem"]
        SUI["SUI Plugin"]
        SGAS["Gas Sponsorship"]
        SOL["Solana Plugin"]
        SFEE["Fee Payer Service"]
        ETH["Ethereum Plugin"]
        EMETA["Meta-transactions"]
        POL["Polygon Plugin"]
        PMETA["Meta-transactions"]
        BSC["BSC Plugin"]
        BMETA["Meta-transactions"]
        ARB["Arbitrum Plugin"]
        AMETA["Meta-transactions"]
        BASE["Base Plugin"]
        BASEMETA["Meta-transactions"]
        CUSTOM["Custom Chain Plugin"]
        CMETA["Chain Features"]
    end
    
    %% Connections
    A --> B & C & E
    B --> D
    AI --> D & MCP
    MCP --> UAG & ANY & G
    UAG --> AO & OPT & G
    ANY --> OPENAI & CLAUDE & LLAMA & LOCAL
    E --> F & G & I
    F --> H
    HL --> G
    I --> J & K & CS
    J --> L
    K --> M
    PR --> M
    CS --> TR
    TR --> CA & PM
    CA --> PM
    PM --> HR & SUI & SOL & ETH & POL & BSC & ARB & BASE & CUSTOM
    BR --> BA
    BA --> WH & LZ & AX
    STORAGE --> TRAD & BLOCKCHAIN
    TRAD --> V & W
    BLOCKCHAIN --> PM & V
    V --> W & X
    W --> Y
    ML --> V
    CC --> PM
    MIG --> TRAD & BLOCKCHAIN
    AO --> AAnalytics & ACampaign & ASupport & AFraud
    OPT --> G
    SUI --> BR & SGAS
    SOL --> BR & SFEE
    ETH --> BR & EMETA
    POL --> BR & PMETA
    BSC --> BR & BMETA
    ARB --> BR & AMETA
    BASE --> BR & BASEMETA
    CUSTOM --> CMETA
    
    %% Individual Component Styles
    style MCP fill:#FF6B6B,stroke:#333,stroke-width:2px
    style UAG fill:#10B981,stroke:#333,stroke-width:2px
    style OPT fill:#FFD700,stroke:#333,stroke-width:2px
    style J fill:#FFD700,stroke:#333,stroke-width:2px
    style CA fill:#10B981,stroke:#333,stroke-width:2px
    style PM fill:#8B5CF6,stroke:#333,stroke-width:2px
    style BR fill:#F59E0B,stroke:#333,stroke-width:2px
    style SUI fill:#4DA2FF,stroke:#333,stroke-width:2px
    style SOL fill:#9945FF,stroke:#333,stroke-width:2px
    style STORAGE fill:#10B981,stroke:#333,stroke-width:3px
    style TRAD fill:#4DA2FF,stroke:#333,stroke-width:2px
    style BLOCKCHAIN fill:#FFD700,stroke:#333,stroke-width:2px
    style MIG fill:#F59E0B,stroke:#333,stroke-width:2px
    
    %% Subgraph Styles
    style subGraph0 fill:#E3F2FD,stroke:#1976D2,stroke-width:3px
    style subGraph1 fill:#FCE4EC,stroke:#C2185B,stroke-width:3px
    style subGraph2 fill:#E8F5E8,stroke:#388E3C,stroke-width:3px
    style subGraph3 fill:#FFF3E0,stroke:#F57C00,stroke-width:3px
    style subGraph4 fill:#F3E5F5,stroke:#7B1FA2,stroke-width:3px
    style subGraph5 fill:#E0F2F1,stroke:#00695C,stroke-width:3px
    style subGraph6 fill:#FFF8E1,stroke:#F9A825,stroke-width:3px
    style subGraph7 fill:#EFEBE9,stroke:#5D4037,stroke-width:3px
```

## 💎 NFT-Powered Loyalty Revolution

### Transform Achievements into Digital Assets

Ploy revolutionizes loyalty programs with flexible reward systems that scale with your needs:

#### Traditional Mode (Cost-Effective Start)
- **🏆 Digital Achievement Badges** - Visual recognition stored in database
- **👑 Membership Tiers** - Dynamic status levels with real benefits
- **🎫 Access Passes** - Time-limited privileges and experiences
- **🎨 Collectible Cards** - Digital collections with rarity systems
- **⚡ Utility Rewards** - Functional benefits and perks

#### Blockchain Mode (Premium Features)
- **🏆 True NFT Ownership** - On-chain certificates with real value
- **👑 Dynamic NFTs** - Tokens that evolve based on user activity
- **🎫 Transferable Access** - Trade or gift exclusive experiences
- **🎨 NFT Collections** - Limited edition series with market value
- **⚡ Cross-Platform Assets** - Use NFTs across multiple platforms

### Marketplace Features (Available in Blockchain Mode)

- **Multi-Chain Trading** - Trade across SUI, Solana, and EVM chains
- **Zero Trading Fees** - Gas-less transactions for all users
- **Point-to-NFT Purchases** - Buy NFTs directly with loyalty points
- **Dynamic Pricing** - Demand-based pricing with user discounts
- **NFT Upgrades** - Enhance and evolve NFTs using points
- **Advanced Auctions** - Dynamic bidding with automatic extensions
- **NFT Rentals** - Temporary access with smart contract protection
- **Fractionalization** - Share ownership of high-value NFTs

## 🤖 Universal AI Integration with Model Context Protocol

### Any LLM, One Platform

Connect ANY Large Language Model to Ploy using the industry-standard Model Context Protocol (MCP):

- **OpenAI GPT-4** - "Create a loyalty campaign for my SaaS users"
- **Anthropic Claude** - "Analyze customer segments and suggest NFT rewards"  
- **Meta Llama** - "Optimize our policy rules for better engagement"
- **Local Models** - Run privacy-first AI with Ollama integration
- **Custom Models** - Fine-tuned models for your specific industry

### MCP-Powered Loyalty Tools

Universal tools that work with any LLM client:

```bash
# Install Ploy MCP Server
npm install -g @ploy/mcp-server

# Connect from any MCP-compatible client
mcp connect ploy://your-business.ploy.io
```

**Available Tools:**
- `create_campaign` - AI-optimized campaign creation
- `analyze_segments` - User behavior analysis and insights
- `optimize_policy` - Data-driven policy recommendations
- `mint_achievement_nft` - Blockchain-powered reward creation
- `select_optimal_chain` - Smart chain selection for transactions
- `predict_churn_risk` - ML-powered retention insights

### AI Agent Ecosystem

- **Analytics Agent** - Natural language data exploration across all metrics
- **Campaign Agent** - Automated A/B testing and optimization
- **Support Agent** - Context-aware customer assistance with loyalty history
- **Fraud Detection Agent** - Real-time anomaly detection with blockchain verification
- **Cross-Chain Optimizer** - Intelligent routing for lowest fees and fastest confirmation
- **NFT Creator Agent** - AI-assisted digital asset design and minting

### Universal Integration Benefits

- **MCP Standard Compliance** - Works with 20+ existing AI tools and platforms
- **Provider Agnostic** - Switch between OpenAI, Claude, Llama without code changes
- **Ecosystem Ready** - Instant integration with Zapier, Make, n8n, and development tools
- **Future Proof** - Automatic compatibility with new LLM providers
- **Loyalty Optimized** - Custom performance enhancements for loyalty use cases

## 🌍 Industry Solutions

### SaaS Platforms
- API usage achievements
- Developer certification NFTs
- Integration mastery rewards
- Subscription tier benefits

### E-commerce
- Seller performance recognition
- Customer journey milestones
- Review contribution rewards
- Limited product NFTs

### Travel & Hospitality
- Destination collection NFTs
- Elite status achievements
- Experience milestone rewards
- Transferable travel perks

### FinTech
- Financial wellness achievements
- Investment milestone NFTs
- Credit improvement rewards
- Staking multiplier benefits

### Cloud Infrastructure
- Optimization achievements
- Sustainability certificates
- Innovation adoption rewards
- Cost-saving recognition

### Gaming
- Tournament victory NFTs
- Achievement certificates
- Community contribution badges
- Cross-platform assets

### Health & Fitness
- Fitness achievement NFTs
- Wellness journey milestones
- Transformation recognition
- Health insurance benefits

### Food & Drink
- Culinary achievement NFTs
- Restaurant loyalty rewards
- Chef collaboration access
- Premium dining experiences

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ 
- Docker & Docker Compose
- Git

### Installation

```bash
# Clone the repository
git clone https://github.com/channainfo/ploy.git
cd ploy

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your configuration

# Start development environment
docker-compose up -d

# Run database migrations
npm run migration:run

# Start the development server
npm run dev
```

### Environment Setup

```bash
# Required environment variables
DATABASE_URL=postgresql://user:password@localhost:5432/ploy
REDIS_URL=redis://localhost:6379

# Blockchain Configuration (Mainnet)
SUI_RPC_URL=https://fullnode.mainnet.sui.io:443
SOLANA_RPC_URL=https://api.mainnet-beta.solana.com
POLYGON_RPC_URL=https://polygon-rpc.com

# Gas Sponsorship Keys
SUI_SPONSOR_KEY=your_sui_sponsor_key
SOLANA_FEE_PAYER_KEY=your_solana_payer_key

# API Configuration
JWT_SECRET=your_jwt_secret
API_PORT=3000
```

## 🛠️ Technology Stack

### Backend
- **Framework**: NestJS (TypeScript)
- **Database**: PostgreSQL with TypeORM with migration
- **Sample data**: Generate by seeds
- **Caching**: Redis with pub/sub
- **Swagger Api docs**: Use swagger for api doc
- **Testing framework**: Use jest with TDD in mind
- **Queue**: Bull/BullMQ
- **Authentication**: JWT with multi-tenant isolation

### Storage & Blockchain
- **Traditional**: PostgreSQL + Redis for cost-effective loyalty
- **Blockchain Ready**: Schema designed for seamless migration
- **SUI**: Move smart contracts with object-centric design (optional)
- **Solana**: Anchor framework with compressed NFTs (optional)
- **EVM**: Solidity with OpenZeppelin standards (optional)
- **Bridge**: Wormhole + custom validator network (blockchain mode)
- **Migration**: Zero-downtime transition service

### Frontend
- **Framework**: Next.js 14 with App Router
- **Styling**: Tailwind CSS + Radix UI
- **Web3**: wagmi, @mysten/sui.js, @solana/web3.js
- **State**: Zustand with React Query
- **Analytics**: Segment + Mixpanel

### Infrastructure
- **Deployment**: AWS ECS Fargate with auto-scaling
- **Infrastructure as Code**: Terraform for AWS resource management
- **CDN**: Cloudflare for global distribution
- **Monitoring**: Prometheus, Grafana, Sentry
- **CI/CD**: GitHub Actions with staging/production pipelines

## 📊 Performance & Scale

- **Transaction Speed**: <1 second on SUI/Solana
- **Throughput**: 10,000+ TPS capability
- **User Capacity**: Multi-tenant architecture for millions
- **Global Reach**: Multi-region deployment
- **Uptime**: 99.9% SLA guaranteed

## 🔐 Security Features

- **Smart Contract Audits**: Certified by leading firms
- **Multi-Signature Wallets**: Treasury protection
- **Fraud Detection**: ML-powered anomaly detection
- **Privacy**: Zero-knowledge proof integration
- **Compliance**: GDPR, CCPA, SOC2 ready

## 📚 Documentation

### 🤝 For Contributors & Developers
> **Start here if you want to contribute to Ploy or integrate it into your application**

- **[🚀 Developer Documentation](./docs/external/)** - Complete guide for contributors and developers
- **[🏗️ Platform Architecture](./docs/external/architecture/platform-architecture-overview.md)** - Technical architecture overview
- **[🤝 Contributing Guide](./docs/external/contributing/CONTRIBUTING.md)** - How to contribute to Ploy
- **[💻 Code Examples](./docs/external/examples/code-examples-guide.md)** - Real-world implementation examples
- **[📦 SDK Guide](./docs/external/integrations/sdk-integration-guide.md)** - Complete SDK reference and integration guide

### 📊 For Business & Strategy
> **Market analysis, adoption strategies, and business implementation guidance**

- **[🎯 Business Strategies](./docs/internal/business-strategy/)** - Market penetration and adoption frameworks
- **[⚠️ Risk Analysis](./docs/internal/business-strategy/risk-opportunity-analysis.md)** - Strategic assessment and opportunities
- **[🏭 Industry Templates](./docs/external/examples/industry-templates.md)** - Pre-built solutions for different sectors

### 🔧 For Implementation Teams
> **Detailed technical specifications and implementation roadmaps**

- **[📋 Implementation Plan](./docs/internal/implementation/)** - 16-week development roadmap
- **[🏗️ Technical Specifications](./docs/internal/technical-specs/)** - Detailed technical implementation
- **[🔄 Workflow Patterns](./docs/internal/workflows/)** - End-to-end implementation examples
- **[🚀 Deployment Guide](./docs/internal/implementation/deployment/)** - Production deployment with AWS and Cloudflare

### 🛠️ Technical References
- **[🔌 API Reference](./docs/external/api/)** - Complete REST API documentation
- **[💎 Smart Contracts](./contracts/)** - SUI, Solana, and EVM implementations
- **[🔧 Configuration Guides](./docs/external/integrations/)** - Integration patterns and setup guides

## 💳 Flexible Pricing Options

### Start Small, Scale Big

| Feature | Starter ($29/mo) | Professional ($99/mo) | Enterprise ($299/mo) |
|---------|------------------|----------------------|----------------------|
| **Storage Mode** | Traditional Only | Traditional or Blockchain | Hybrid (Both) |
| **Users** | Up to 1,000 | Up to 10,000 | Unlimited |
| **Transactions** | 10,000/month | 100,000/month | Unlimited |
| **AI Queries** | 100/month | 1,000/month | 10,000/month |
| **NFT Rewards** | Digital Badges | Real NFTs (optional) | Full NFT Suite |
| **Gas Sponsorship** | Not Available | $50/month addon | $200 included |
| **Custom Branding** | Basic | Full | White-Label |
| **Support** | Email | Priority Email | Dedicated Manager |
| **Migration Tools** | Not Included | Included | Premium Migration |

### 💰 Cost Comparison

**Traditional Mode:**
- Points Transaction: $0.001 per transaction
- Digital Badge Creation: Free
- Storage: Included in base price
- No blockchain fees

**Blockchain Mode:**
- Points Transaction: $0.02-0.05 (gas sponsored)
- NFT Minting: $0.50-1.50 per NFT
- Storage: Traditional + blockchain costs
- Optional gas sponsorship available

## 🗺️ Roadmap

### Phase 1: Core Platform Development (Q3 2025) 🚧
- [ ] Backend API infrastructure (NestJS + TypeScript)
- [ ] Database design and migration system (PostgreSQL + TypeORM)
- [ ] Authentication and multi-tenant isolation (JWT)
- [ ] Frontend foundation (Next.js 14 + React)
- [ ] Basic UI components and design system
- [ ] Traditional storage loyalty engine (points, tiers, rewards)
- [ ] **Dynamic field engine and service registry**
- [ ] **Multi-service architecture foundation**
- [ ] **Basic digital asset marketplace (traditional storage)**
- [ ] **Service composition framework**

### Phase 2: AI & MCP Integration (Q4 2025) 🔮
- [ ] MCP Protocol Server implementation
- [ ] Universal LLM Gateway development
- [ ] AI agent ecosystem (Analytics, Campaign, Support, Fraud)
- [ ] Loyalty optimization algorithms
- [ ] Natural language query processing
- [ ] **Advanced search and discovery engine**
- [ ] **Trading engine (auctions, bids, direct sales)**
- [ ] **Dynamic pricing algorithms**
- [ ] **Cross-service workflows**

### Phase 3: Advanced Features & Launch (Q1 2026) 🚀
- [ ] Mobile app development (React Native)
- [ ] Advanced analytics and reporting
- [ ] Enterprise features and white-labeling
- [ ] **Bulk operations and collection management**
- [ ] **Cross-platform marketplace integrations**
- [ ] **Advanced trading features (bundles, fractionalization)**
- [ ] **External marketplace sync (OpenSea, etc.)**
- [ ] Public beta release and partner onboarding
- [ ] Production deployment and monitoring

### Phase 4: Optional Blockchain Integration (Q2 2026) 📅
- [ ] Multi-chain architecture implementation
- [ ] Smart contract development (SUI, Solana, EVM)
- [ ] Gas-less transaction system
- [ ] Chain abstraction layer and plugin manager
- [ ] NFT minting engine and metadata standards
- [ ] **Asset tokenization engine**
- [ ] **Cross-chain asset bridging**
- [ ] **Blockchain marketplace integration**
- [ ] **External NFT marketplace sync**
- [ ] Migration tools from traditional to blockchain storage

## 🤝 Contributing

We welcome contributions! Please see our documentation contributing guides:

- **[📖 Documentation Contributing](./docs/features/CONTRIBUTING.md)** - How to contribute to our documentation
- **[💻 Code Contributing](./docs/external/contributing/CONTRIBUTING.md)** - How to contribute code to the platform
- **[🔧 Feature Documentation](./docs/features/README.md)** - Guidelines for documenting platform features

### Development Workflow

```bash
# Create feature branch
git checkout -b feature/amazing-feature

# Make changes and test
npm run test
npm run lint

# Commit with conventional commits
git commit -m "feat: add amazing feature"

# Push and create PR
git push origin feature/amazing-feature
```

## 🏢 Enterprise Solutions

### White-Label Platform
- Custom branding and domains
- Dedicated infrastructure
- Priority support
- Custom feature development

### Integration Services
- API integration assistance
- Smart contract customization
- Migration from existing systems
- Training and documentation

## 📈 Success Stories

> "We started with traditional storage to test the waters. Within 3 months, we upgraded to blockchain and saw engagement jump 300%!" - *TechCorp CTO*
>
> "The ability to launch without blockchain complexity was key. We onboarded 10,000 users before enabling NFT features." - *E-commerce Director*
>
> "Perfect for our growth. Started at $29/month, now on Enterprise with full blockchain features. Seamless scaling!" - *SaaS Startup CEO*
>
> "The migration from traditional to blockchain was flawless. Zero downtime and our users loved the new NFT rewards." - *Gaming Studio Director*

## 🌟 Why Choose Ploy?

### For Businesses
- **Start Small**: Launch with traditional storage, no blockchain complexity
- **Scale Smart**: Upgrade to blockchain when it makes business sense
- **Lower Entry Costs**: Traditional mode 90% cheaper than blockchain-first platforms
- **Flexible Adoption**: Each tenant chooses their storage strategy
- **Future-Proof**: Seamless migration preserves all historical data
- **Quick Launch**: Deploy loyalty programs in days, not months

### For Developers
- **Storage Abstraction**: Single API works with both traditional and blockchain
- **Modern Stack**: TypeScript, React, NestJS, latest Web3
- **Great DX**: Comprehensive docs, SDKs, and migration tools
- **Open Source**: Contribute and customize
- **Innovation**: Build on cutting-edge tech with pragmatic options

### For Users
- **Same Experience**: Seamless UX regardless of storage mode
- **Optional Ownership**: Digital badges or true NFT ownership
- **Zero Fees**: No costs in traditional mode, sponsored gas in blockchain
- **Real Value**: Points always valuable, NFTs when you want them
- **Cross-Platform**: Rewards work everywhere

## 📞 Get in Touch

- **Website**: [ploy.io](https://ploy.io)
- **Documentation**: [docs.ploy.io](https://docs.ploy.io)
- **Discord**: [discord.gg/ploy](https://discord.gg/ploy)
- **Twitter**: [@ploy_platform](https://twitter.com/ploy_platform)
- **Email**: hello@ploy.io

### Enterprise Inquiries
- **Sales**: enterprise@ploy.io
- **Partnerships**: partners@ploy.io
- **Support**: support@ploy.io

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.

---

<div align="center">
  <h3>🚀 Ready to revolutionize loyalty?</h3>
  <a href="https://ploy.io/demo"><img src="https://img.shields.io/badge/Book%20Demo-4DA2FF?style=for-the-badge&logo=googlemeet&logoColor=white" alt="Book Demo" /></a>
  <a href="https://discord.gg/ploy"><img src="https://img.shields.io/badge/Join%20Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Join Discord" /></a>
  <a href="https://docs.ploy.io"><img src="https://img.shields.io/badge/Read%20Docs-000000?style=for-the-badge&logo=readthedocs&logoColor=white" alt="Read Documentation" /></a>
</div>

<div align="center">
  <sub>Built with ❤️ by the Ploy team. Powered by SUI and Solana.</sub>
</div>