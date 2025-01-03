# Coming Soon

# Project Overview

Dial.WTF revolutionizes Web3 communication with wallet-to-wallet audio
calls, interactive Spaces, and monetization tools, enabling users to
connect, flex, and earn seamlessly on-chain. The platform combines
low-latency, scalable peer-to-peer calls with multiple monetization
options like streaming payments and Space auctions while integrating
NFTs and PFPs for personalized branding. Offering on-chain transparency
and user-friendly design, Dial.WTF empowers users with insights into
wallet interactions, audience metrics, and revenue streams for smarter
engagement in the decentralized community.

# Codebase and Deployment Architecture

-   **Frontend:** React + Vite deployed on Replit.
-   **Backend:** Express.js server deployed on Replit.
-   **Database:** Neon Postgres with Drizzle ORM.

Roadmap:

-   **State Management:** Establish a cohesive client-server state management strategy for a straightforward / seamless developer experience.

# Wallet Connection

-   **Universal Wallet Connect:** Unified interface for wallet integration across blockchains.
-   **Wallet Integration:**
    -   EVM (Ethereum, Base, others) using RainbowKit, Wagmi, and ethers.js.
    -   Solana via \@solana/wallet-adapter-react.
    -   Dogecoin support (coming soon).
-   **Session and Identity Management:**
    -   SIWE (Sign-In With Ethereum) to authenticate and verify wallet ownership.
    -   Store SIWE sessions in the Express.js backend to establish user identity and enable database access.

Roadmap:

-   Connect your ENS username
-   Create your Profile Page, edit your PFP and username, etc.

# P2P Calling Experience

-   **WebRTC Implementation:**
    -   Use Peer.js for wallet-to-wallet WebRTC audio calls.
    -   Link user wallet addresses with Peer IDs in Neon Postgres for address-to-Peer ID resolution.
-   **Call Management:**
    -   Users can make calls by entering an address, and the recipient can accept or decline.
    -   Maintain call lifecycles over WebRTC and log call history in Neon Postgres.
-   **Address Book:** Store contact information in the database for quick access.
-   **Premium Access NFTs:** Buy a subscription NFT on unlock protocol for access to more features.

In-Progress (Standing By):

-   **Pay-By-Second:** Integrate Superfluid Finance for streaming payments during active calls.

Roadmap:

-   **Call Forwarding:** Integrate Onesignal to push incoming call notifications. (Paid feature)
-   **Pay-Per-Call:** Allow users to charge a fixed Ethereum fee for initiating a call.
-   **Customization:** Offer NFTs for personalized dial tones and ringtones, and skins for the user interface.

# Spaces Experience

**Project Status:** *Under Development*

## Core Spaces Infrastructure

-   **SFU Integration:**
    -   Use scalable SFU solutions like 100ms or Jitsi to handle up to 10k participants per space and 100 - 1,000 concurrent spaces.
    -   Build client-server wrappers to manage the lifecycle of spaces and participant roles (host, speaker, listener).
-   **Space Functionality:**
    -   Implement core audio space features: host controls to start, invite, or end spaces, hear speakers, mute/unmute, and request speaking rights.
    -   Optional feature: Audio recording and playback for spaces.

## Monetization and Gating

-   **Entry Fees:**
    -   Allow hosts to charge Ethereum entry fees for access to spaces.
    -   Provide the option for free spaces.
-   **NFT Gating:**
    -   Restrict access to specific NFT holders, enabling exclusive spaces for communities or collectors.

## Advanced Space Features

-   **Text Chat / Trollbox:** Realtime chat with emojis etc. so the listeners can participate, meme, troll, throw tips, etc. (Like Twitch)
-   **Space Merging:** Enable two spaces to combine, merging participants and features into a single room.
-   **Ownership Transfers:**
    -   Allow spaces to be auctioned or purchased, transferring host privileges and space management rights.
-   **Customizations:** Extend monetization options and interface personalization for space hosts.

# Features Roadmap

-   Connect your Ethereum/Base Wallet (EVM compatible)
-   Connect your Solana Wallet
-   Wallet-to-Wallet Calling
-   Show the Total Number of Dials
-   Cross-Chain Wallet-to-Wallet Calling
-   Address Book
-   Profile PFP
-   ENS Integration
-   Push Notifications (Receiving a Call)
-   Call History
-   Voicemail
-   Farcaster Frame (Call Me / Calling Card, Spaces)
-   Charge Callers to Call You
-   Charge by the Minute
-   Custom Dial Tones (ringtones)
-   Custom Skin
-   Audio Spaces
-   NFT-Gated Spaces
-   Pay-to-Join Spaces
-   Trollbox in Spaces
-   Display Total Net Worth of Spaces
-   Buy-Out a Space
-   Merge Spaces
-   One Million Dolars? Buy your own "Real Number"! Burners? SIP Trunking!
