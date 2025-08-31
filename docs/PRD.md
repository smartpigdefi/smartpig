# Product Requirements Document (PRD)
## Smart Pig - DeFi Simplificado

---

## 1. Executive Summary

### 1.1 Product Vision
Smart Pig is a gamified DeFi platform that democratizes yield farming for Brazilian users by providing a seamless PIX-to-USDC investment experience with 7-10% annual returns. The platform transforms complex DeFi operations into an intuitive, pig-themed interface where users watch their virtual pig grow as their investments prosper.

### 1.2 Mission Statement
"Se qualquer pessoa usa sem ajuda, criamos a solução certa" (If anyone can use it without help, we've created the right solution)

### 1.3 Target Market
- **Primary**: Brazilian retail investors with R$10K+ in savings
- **Secondary**: DeFi-curious users seeking simplified crypto investment
- **Market Size**: R$1.2 trillion Brazilian savings market

---

## 2. Problem Statement

### 2.1 Market Pain Points
- **R$1.2 trillion** sitting in Brazilian savings accounts earning only 6% annually
- **86%** of Brazilians want alternatives to traditional savings
- **Only 3%** of population accesses DeFi due to complexity
- **95%** find traditional DeFi too complex to use

### 2.2 User Friction Points
- Complex wallet management and seed phrases
- Unfamiliar blockchain terminology
- High barriers to entry for crypto investment
- Lack of Brazilian payment integration (PIX)
- Regulatory uncertainty in DeFi

---

## 3. Solution Overview

### 3.1 Core Value Proposition
"DeFi Invisível" - A completely transparent DeFi experience where users simply deposit via PIX and earn 7-10% annually in USDC without needing to understand blockchain complexity.

### 3.2 Key Differentiators
- **Biometric Authentication**: Face ID/Touch ID/Windows Hello integration
- **PIX Native**: Instant Brazilian payment integration
- **Gamified Interface**: Pig evolution system based on investment levels
- **Regulatory Compliance**: Full Brazilian financial regulation compliance
- **Stellar Blockchain**: Fast, low-cost transactions with smart contracts

---

## 4. Product Features

### 4.1 Authentication System
**Feature**: Stellar Passkeys Authentication
- **Description**: WebAuthn-based biometric authentication using secp256r1 protocol
- **User Flow**: 
  1. User creates account with biometric verification
  2. Smart wallet automatically generated on Stellar network
  3. No passwords or seed phrases required
- **Technical Requirements**:
  - WebAuthn API integration
  - Stellar SDK for wallet creation
  - secp256r1 cryptographic algorithm
  - Cross-platform biometric support

### 4.2 Gamified Investment Interface
**Feature**: Pig Evolution System
- **Description**: Visual representation of investment growth through pig character evolution
- **Levels**:
  - 🐷 **Level 1** (R$0-500): Beginner pig
  - 🐽 **Level 2** (R$500-2K): Growing pig
  - 🐖 **Level 3** (R$2K-5K): Prosperous pig
  - 🐷👑 **Level 4** (R$5K-15K): Rich pig
  - 🐷💎 **Level 5** (R$15K+): Magnate pig
- **Features**:
  - Real-time balance updates
  - Motivational messages on level-ups
  - Visual animations and effects
  - Progress indicators

### 4.3 PIX Integration
**Feature**: Native Brazilian Payment System
- **Description**: Seamless BRL to USDC conversion via PIX
- **User Flow**:
  1. User enters deposit amount
  2. QR code generated instantly
  3. PIX payment processed
  4. Automatic BRL→USDC conversion
  5. Funds available for yield farming
- **Technical Requirements**:
  - PIX API integration
  - QR code generation
  - Real-time payment status
  - Automatic currency conversion
  - Stellar Anchor integration

### 4.4 Yield Farming Dashboard
**Feature**: Real-time Investment Tracking
- **Description**: Live monitoring of investment performance and earnings
- **Features**:
  - 7-10% annual yield display
  - Real-time earnings calculation
  - Historical transaction view
  - Performance analytics
  - Withdrawal functionality

### 4.5 Demo Mode
**Feature**: Presentation-Ready Demo Environment
- **Description**: Accelerated demo mode for presentations and marketing
- **Features**:
  - Pre-configured R$2,400 starting balance
  - Accelerated earnings simulation
  - Instant PIX processing
  - Automatic level progression
  - Visual impact optimization

---

## 5. Technical Architecture

### 5.1 Frontend Stack
- **Framework**: React 18 with TypeScript
- **Styling**: CSS3 with modern animations
- **Authentication**: WebAuthn API for Passkeys
- **Blockchain**: Stellar SDK integration
- **Design**: Mobile-first responsive design

### 5.2 Backend Stack
- **Framework**: NestJS with TypeScript
- **Blockchain**: Stellar Network integration
- **Payment**: PIX integration via Stellar Anchors
- **Real-time**: WebSockets for live updates
- **Security**: WebAuthn server-side validation

### 5.3 Blockchain Infrastructure
- **Network**: Stellar Mainnet
- **Smart Contracts**: Soroban for yield pools
- **Stablecoin**: USDC as base currency
- **Yield Protocol**: Aquarius Protocol integration
- **Security**: Multi-signature wallets

---

## 6. User Experience Requirements

### 6.1 Onboarding Flow
1. **Welcome Screen**: Introduction to Smart Pig concept
2. **Biometric Setup**: Passkey creation with device biometrics
3. **Wallet Creation**: Automatic Stellar smart wallet generation
4. **First Deposit**: Guided PIX deposit tutorial
5. **Dashboard Introduction**: Pig interface explanation

### 6.2 Core User Journeys
**Deposit Flow**:
1. User clicks "Depositar" button
2. Enters amount (minimum R$10)
3. PIX QR code generated
4. User scans with banking app
5. Payment confirmed automatically
6. Pig grows and level-up animation plays

**Withdrawal Flow**:
1. User clicks "Sacar" button
2. Enters withdrawal amount
3. Confirms transaction
4. Funds converted to BRL
5. PIX transfer initiated
6. Confirmation received

### 6.3 Accessibility Requirements
- **WCAG 2.1 AA** compliance
- **Mobile-first** responsive design
- **Biometric accessibility** for users with disabilities
- **High contrast** mode support
- **Screen reader** compatibility

---

## 7. Business Requirements

### 7.1 Revenue Model
- **Yield Spread**: 1-2% spread on yield farming returns
- **Transaction Fees**: 0.1% on deposits/withdrawals
- **Premium Features**: Advanced analytics for high-value users

### 7.2 Compliance Requirements
- **LGPD Compliance**: Brazilian data protection law
- **BCB Regulations**: Central Bank of Brazil compliance
- **KYC/AML**: Know Your Customer and Anti-Money Laundering
- **Tax Reporting**: Automatic tax documentation generation

### 7.3 Partnership Strategy
- **Banco do Brasil**: "Poupança Digital BB" partnership
- **Sicredi**: "Porquinho Cooperativo" integration
- **Stellar Foundation**: Blockchain infrastructure support
- **Aquarius Protocol**: Yield pool management

---

## 8. Success Metrics

### 8.1 User Metrics
- **User Acquisition**: 10K users in first 6 months
- **Retention Rate**: 70% monthly active users
- **Average Investment**: R$5,000 per user
- **Conversion Rate**: 25% from demo to real investment

### 8.2 Business Metrics
- **Total Value Locked (TVL)**: R$50M in first year
- **Revenue**: R$2M annual recurring revenue
- **Market Share**: 5% of Brazilian DeFi market
- **Customer Satisfaction**: 4.5/5 rating

### 8.3 Technical Metrics
- **Uptime**: 99.9% availability
- **Transaction Speed**: <3 seconds for PIX deposits
- **Security**: Zero security incidents
- **Performance**: <2 second page load times

---

## 9. Risk Assessment

### 9.1 Technical Risks
- **Blockchain Volatility**: Stellar network stability
- **Smart Contract Security**: Yield pool vulnerabilities
- **Biometric Failures**: Authentication system reliability
- **PIX Integration**: Payment system dependencies

### 9.2 Business Risks
- **Regulatory Changes**: Brazilian crypto regulations
- **Market Volatility**: Crypto market fluctuations
- **Competition**: Traditional banks entering DeFi
- **User Adoption**: Market education challenges

### 9.3 Mitigation Strategies
- **Multi-chain Support**: Backup blockchain networks
- **Security Audits**: Regular smart contract reviews
- **Regulatory Monitoring**: Active compliance tracking
- **User Education**: Comprehensive onboarding materials

---

## 10. Development Roadmap

### 10.1 Phase 1: MVP (Completed)
- ✅ Gamified interface implementation
- ✅ Mocked Passkey authentication
- ✅ Simulated PIX integration
- ✅ Design system completion

### 10.2 Phase 2: Integration (Current)
- 🔄 NestJS backend development
- 🔄 Real PIX integration via Stellar Anchors
- 🔄 Functional smart wallets
- 🔄 WebSocket real-time updates

### 10.3 Phase 3: Production (Q3 2025)
- 🚀 AWS/Vercel deployment
- 🚀 End-to-end testing completion
- 🚀 Security audit and certification
- 🚀 Official launch and marketing

### 10.4 Phase 4: Scale (Q3-Q4 2025)
- 📈 Partnership integrations
- 📈 Advanced analytics features
- 📈 Mobile app development
- 📈 International expansion

---

## 11. Technical Specifications

### 11.1 API Endpoints
```
POST /api/auth/passkey/create
POST /api/auth/passkey/authenticate
POST /api/stellar/pix-deposit
GET /api/stellar/balance/{accountId}
POST /api/stellar/withdraw
GET /api/yield/earnings/{accountId}
```

### 11.2 Database Schema
```sql
Users:
- id, public_key, contract_id, created_at, updated_at

Transactions:
- id, user_id, type, amount, status, tx_hash, created_at

PIXPayments:
- id, user_id, amount, pix_key, qr_code, status, expires_at
```

### 11.3 Security Requirements
- **Encryption**: AES-256 for data at rest
- **Authentication**: WebAuthn FIDO2 standard
- **Authorization**: JWT tokens with short expiration
- **Audit Logging**: Complete transaction trail
- **Rate Limiting**: API abuse prevention

---

## 12. Conclusion

Smart Pig represents a paradigm shift in DeFi accessibility, combining cutting-edge blockchain technology with intuitive user experience design. The platform's success hinges on its ability to make complex financial instruments accessible to everyday Brazilian users while maintaining the security and transparency expected in DeFi applications.

The gamified approach, combined with native PIX integration and biometric authentication, creates a unique value proposition that addresses the core friction points preventing mainstream DeFi adoption in Brazil. With proper execution of the outlined roadmap and risk mitigation strategies, Smart Pig has the potential to capture a significant share of the Brazilian DeFi market and establish itself as the go-to platform for simplified crypto investment.

---

## Document Information

- **Version**: 1.0
- **Last Updated**: August 2025
- **Author**: Smart Pig Development Team
- **Status**: Draft for Review
- **Next Review**: September 2025
