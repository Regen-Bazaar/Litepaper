# Regen Bazaar Phases for Implementation (Detailed Roadmap)

---

## Phase #1: Core Functionality Development

### 1. NGO & Community Dashboard (Profile) and Tokenization Page

#### **Objective**
Enable NGOs and communities to manage their profiles and convert their real-world impact data (RWI Data) into blockchain-based digital assets (Impact Products).

#### **Key Features & Tasks**

- **NGO & Community Dashboard (Profile):**
  - **Profile Management & Statistics:**
    - Develop a secure dashboard where NGOs and communities manage their profiles and track impact metrics.
  - **Dashboard Contents:**
    - **Created but Not Listed Impact Products:** Display Impact Products that have been created but not yet listed for sale.
    - **Listed for Sale Impact Products:** Showcase Impact Products currently available for purchase on the marketplace.
    - **Pending Verification Section:** Add a section on the seller profile that displays Impact Products pending verification.
  - **Statistical Metrics:**
    - **Impact Products Created:** Total number of Impact Products created by the NGO/community.
    - **Impact Products Sold:** Number of Impact Products sold.
    - **Amount $$$ Earned from IP Sales:** Total revenue generated from Impact Product sales.
    - **Quadratic Funding (QF) Participated:** (To be integrated in later phases.)
    - **Proposals Submitted:** (To be integrated in later phases.)
  - **Secure Registration & Identity Verification:**
    - Leverage web3 wallets (e.g., Unicorn.eth for EVM) for user authentication.
    - Collect additional user/organization data during registration integrated within the dashboard.

- **Tokenization Page:**
  - **Data Submission Interface:**
    - Create an intuitive interface for NGOs/communities to upload impact data (e.g., cleanups, reforestation, workshops) with attachments and images.
    - Design this page based on the current landing page RWI data submission form.
    - Check user flow on Canva for logic.
  - **Impact Data Processing & Tokenization:**
    - **Data Validation:**  
      Conduct manual or basic automated checks to ensure authenticity and accuracy of submitted RWI data.  
      *(Note: In later phases, automatic validation will be performed by decentralized validators as described in Phase #2.)*
    - **Smart Contract Development (Impact Product Factory):**
      - Create NFT collections based on input data with a varying number of NFT tiers.
    - **Open Source Solutions:**  
      Explore existing open source solutions (e.g., Hypercerts) to accelerate development.
    - **Auto-Generated Images (With a Manual Creation Option):**
      - Integrate AI solutions (e.g., Midjourney) to auto-generate images relevant to the uploaded RWI data—presenting the impact beautifully for buyers.
      - Allow for manual creation of images as an alternative in the early stage.
      - Use Impact Value & Price to determine token properties.
      - Split assets into 2 streams (90% to the creator, 10% to Regen Bazaar).
      - Implement a royalty structure (5% to the creator, 5% to Regen Bazaar).
      - Apply a zero-mint approach (limited supply).
      - Allow open collections for mint (listing) via IP creator confirmation.
      - Ensure a closed data framework.
  - **Blockchain Integration:**
    - Deploy on Stellar, Supra, and EVM chains (e.g., Celo).
  - **Pending Verification & Admin Review [Currently Planned Via Air Table]:**
    - **Pending Verification Section for Seller Profile:**  
      Incorporate a section in seller profiles showing Impact Products pending verification.
    - **Admin Account Page for Pending Verification:**  
      Develop an admin dashboard for manual review of RWI data submissions prior to the launch of decentralized validators and automated processing frameworks.
  - **Future Automated Processing (Later Phases) [Phase 2 Once Calculation is Decided]:**
    - In subsequent phases, integrate an automated RWI Data Processing framework that automatically processes user input to derive:
      - **Impact Value**
      - **Price**  
    This framework will utilize formula-based AI or rule-based approaches incorporating ACDM, ESM, and PIM multipliers, along with AI-generated images and community validation.

---

### 2. Marketplace

#### **Objective**
Provide a curated marketplace where retail buyers can explore and purchase Impact Products.

#### **Key Features & Tasks**

- **Gallery:**
  - Build a gallery with filtering and search capabilities to allow users to purchase Impact Products.
- **Seller Profile Link:**
  - Enable users to click on an Impact Product creator's name to showcase all Impact Products listed for sale by that seller.  
  *(Note: Consider exploring existing open source marketplace solutions for partial integration, e.g., thirdweb.)*
- **Display Detailed Product Views:**
  - Display detailed product views with impact metrics, descriptions, and visuals.
- **Transaction Flow:**
  - Develop an end-to-end purchasing process with integrated on-chain transactions.
- **Buyer Dashboard (Profile):**
  - Design a comprehensive dashboard that shows:
    - Purchased Impact Products
    - Staked $REBAZ tokens and staked Impact Products
    - **Stats including:**
      - RWI Rank
      - Voting power ($voREBAZ)
      - Amount of staked Impact Products
      - Average APY% for staked Impact Products
      - Amount of staked $REBAZ tokens
      - Average APY for staked $REBAZ tokens
- **Leaderboard for Buyers & Sellers:**
  - **For Buyers:**
    - **Total Impact Value Purchased:** Rank buyers by the cumulative impact value of all the Impact Products they have bought.
    - **$REBAZ Rewards Earned:** Display the total rewards earned from staking and purchasing.
    - **RWI Rank:** Reflect the buyer's overall real-world impact engagement.
    - **Amount Rewards Distributed to RWI Projects via QFs (Donors Rating):** Show the total rewards that buyers have contributed or distributed to RWI projects through Quadratic Funding rounds.
    - **Referrals Rating:** Rank buyers based on the number of successful referrals they have made.
  - **For Sellers:**
    - **Total Revenue from IP Sales:** Rank sellers by the total revenue generated from selling their Impact Products.
    - **Impact Products Sold:** Display the total number of Impact Products sold.
    - **Average Impact Value per Product:** Present a metric reflecting the average impact value per product.

---

### 3. Rewards System

#### **Objective**
Reward buyers exclusively through the staking of Impact Products by launching and managing the $REBAZ token as the core incentive mechanism.

#### **Key Features & Tasks**

- **$REBAZ Token Launch:**
  - **Token Minting & Tokenomics:**
    - Develop and deploy the $REBAZ token smart contract according to the defined tokenomics.
    - Set up the initial token supply, distribution schedule, and reward pool parameters.  
      *(Note: Detailed tokenomics are available in an existing document (v.1) and will be updated before tasks close.)*
- **Integration with Rewards Distribution:**
  - Integrate the $REBAZ token into the rewards system so that tokens are minted and distributed automatically based on staking activities.
  - Ensure that the token launch aligns with the overall reward strategy for staking Impact Products.
- **Token Rewards Distribution:**
  - Implement smart contract logic to distribute $REBAZ tokens based solely on staking activities involving Impact Products.
- **Staking Mechanics:**
  - Enable users to stake Impact Products, with functions to:
    - **Stake to Get APY:** Stake Impact Products to earn an annual percentage yield.
    - **Lock to Increase Rewards and Voting Power:** Allow users to lock their assets to boost reward multipliers and increase voting power on platform proposals.
    - **Claim Your Reward:** Allow users to view the amount of $REBAZ tokens available for claim and then claim those rewards.
    - **Withdraw Impact Products (IP):** Enable the withdrawal of staked Impact Products.
- **Future Functionality:**
  - In later phases, integrate the ability for users to distribute their rewards to projects via Quadratic Funding (QF).

---

### 4. Enhanced User Engagement & Social Features – Early Implementation

#### **Objective**
Lay the groundwork for social engagement and network growth with simple, early-stage features.

#### **Key Features & Tasks**

- **Guided Creation Flow:**
  - Implement a basic step-by-step wizard that guides creators through the Impact Product creation process.
- **Follow Creators:**
  - Enable users to follow creators and receive updates on new Impact Products.
- **Social Media Sharing:**
  - Integrate simple social media sharing buttons for creators to promote their Impact Products externally and for users to share their marketplace activities or impact achievements.
- **Simplified Account Creation:**
  - Allow users to sign up using existing social media accounts (via OAuth) to streamline onboarding and encourage social engagement.
