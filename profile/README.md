## AuctionClub Project Proposal
### [Project Website](https://auctionclub.github.io/auction_frontend/)
### I. Overview

AuctionClub is a smart contract-based auction platform that provides traders with a fair and reliable auction environment. The platform currently supports two auction modes: English auction and Dutch auction. It also offers a variety of trading rules that sellers can freely combine. Additionally, the platform implements an incentive mechanism to provide positive feedback to bidders. Active participation in bidding can earn bidders auction shares and extract huge profits.

### Project Introduction
#### 1. Starting Auction

1. **Login and Connect Wallet**:
   - Auctioneers connect their wallet address through a plugin wallet or by scanning a QR code for authorization.
   - The platform displays all NFTs under this address for the seller to choose for auction.

2. **Select Auction Mode**:
   - Sellers can choose between two auction modes: English auction or Dutch auction.

#### 2. English Auction

1. **Create Auction**:
   - Sellers select the NFTs for auction and set the starting price, starting time, and bidding interval after each bid.

2. **Bidding Mechanism**:
   - Bidders who bid repeatedly only need to add the difference on top of their initial bid, simplifying the bidding process.
   - Each bid increment must be at least 5% of the starting price.

3. **Incentive Mechanism**:
   - After the auction ends, apart from the successful bidder, other participants will receive 3% of the final price as a reward, distributed according to their bidding funds. The accumulated reward will be added to the balance of the participants who bid when the auction ends.

4. **Fund Handling**:
   - 2% of the final bid price is injected into the fund pool as a platform fee.

#### 3. Dutch Auction

1. **Create Auction**:
   - Sellers select the NFTs for auction and set the starting price, reserve price, starting time, price decay interval, decay amount, and reserve time after reaching the reserve price.
   - The price decay interval must be less than 10 minutes, the decay amount must be greater than 5% of the starting price minus the reserve price, and the reserve time must be less than 20 minutes.

2. **Bidding Mechanism**:
   - After the auction starts, the price of the NFT will decay over time. Bidders can bid when the price reaches their expected price.

3. **Incentive Mechanism**:
   - This auction mode attracts buyers willing to wait for the price to drop to their expected price, while also prompting some buyers to decide to purchase when the price is high to avoid missing out on the item.

4. **Fund Handling**:
   - The platform charges a 3% fee on the transaction amount.

#### 4. End of Auction

1. After the auction ends, the changes in funds for bidders and sellers will be recorded in the statement. Bidders who successfully bid will receive the NFT, and sellers will receive ETH, which will be recorded in their personal balance. They can view their balance in the personal center and withdraw it. The ETH will be sent from the fund pool to their wallet after withdrawal.

### Expected Effects

By introducing an incentive mechanism for auctions, the platform expects to attract more bidders, increase the activity and volume of auctions. Meanwhile, the setting of the pledging mechanism and platform service fees will ensure the security and sustainable operation of the platform.

### Future Development

1. **Feature Expansion**:
   - Add more auction modes and incentive mechanisms to meet the needs of different users.

2. **Cross-chain Compatibility**:
   - Support NFT auctions on more blockchain networks.

3. **Ecosystem Building**:
   - Develop an NFT ecosystem beyond auctions, such as NFT pledging, lending, etc., to enhance the overall value of the platform.

AuctionClub is committed to providing users with a high-quality auction experience and aims to become a leader in the auction industry through innovative auction models and intelligent auction processes.
