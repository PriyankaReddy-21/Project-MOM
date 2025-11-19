# Project Mom 👩🏻

A simplified UX layer on top of MetaMask that makes cross-border crypto remittances as easy as sending money on Google Pay.

## Overview

India is among the world’s largest contributors to global remittance flows, yet traditional cross-border transfers remain slow (1–3 days) and expensive (3–6% in fees). While web3 wallets like MetaMask solve speed and cost challenges, mainstream users struggle with crypto-native concepts such as wallet addresses, gas fees, networks, and tokens.

Project Mom aims to bridge this gap by providing a simple interface that sits on top of Metamask enabling simpler cross-border payments for mainstream users.

## Current Situation

- Remittance fees are high (3–6% including FX).
- Settlement is slow (1–3 days).
- Crypto wallets like MetaMask expose technical details (addresses, gas, tokens).
- India has no widely adopted mainstream-friendly crypto remittance UX layer despite huge demand.

## Pain Point

Non-technical users like my mom can easily use Google Pay but cannot use MetaMask due to its complexity.
This UX friction prevents blockchain-based remittances from reaching mainstream users.

## Proposed Solution

A simple UX layer that sits on top of MetaMask and handles complexity on behalf of the user.

The project aims to :

- Convert user friendly interactions like “Send ₹1000 to Harsh” into the required blockchain transactions.
- Hide wallet addresses, gas fees, and crypto-native complexity and handle them at the backend.
- Enable recipients to transact directly via MetaMask or project-mom interface, as they prefer.

Note : This does not aim to replace MetaMask. It simply packages it in a package which non-technical users can use easily.

## Objectives / Goals

### Stage 1 : MVP
- Allow a non-technical user to send or receive tokens using a simple form-based UI.
- No direct exposure to wallet addresses, gas fees, or networks.

#### Measurable Impact
- Widen adoption of Metamask wallet by main-stream users specially in India.
- Reduce cost from ~3–6% → target < 2%
- Reduce settlement time from days → minutes

### Future Vision
- Mobile app
- Trusted contacts address book
- Indian language support
- Fiat on/off ramps (₹ ↔ USDC)
- Gas-less transactions (ERC-4337)

## Architecture (High Level)

Mainstream User ↔ Mom UI (Frontend) ↔ Middleware (Python + web3.py) ↔ MetaMask SDK ↔ Blockchain
