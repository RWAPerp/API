# Bridging Assets to X Layer

### What Is X Layer?

X Layer is an Ethereum Layer 2 network launched by OKX. Following the “PP Upgrade” in August 2025, X Layer migrated to an enhanced OP Stack architecture and integrated with Polygon AggLayer for cross-chain settlement.

With throughput of up to 5,000 transactions per second and extremely low transaction fees, X Layer is designed to support DeFi, payment, and real-world asset applications.

### X Layer Network Information

* Network Name: X Layer Mainnet
* Chain ID: 196
* Native Gas Token: OKB
* RPC URL: https://rpc.xlayer.tech

### Preparation Before Bridging

Before starting the bridging process, make sure you have completed the following preparations.

#### 1. Prepare a Web3 Wallet

We recommend using the OKX Web3 Wallet, available through the OKX App, web interface, or browser extension. It provides native support for X Layer and includes optimized cross-chain routing.

You may also use other EVM-compatible wallets, such as MetaMask, by manually adding the X Layer network with Chain ID 196.

#### 2. Prepare Assets on the Source Network

Make sure your wallet contains enough assets on the source network, such as Arbitrum, Optimism, Ethereum, or another supported network.

Assets commonly bridged to X Layer include USDT, USDC, and ETH.

#### 3. Prepare Gas on the Source Network

The bridging transaction must first be submitted on the source network. Therefore, you need enough of the source network’s native token to pay the transaction fee.

For example:

* Bridging from Ethereum requires ETH for Gas.
* Bridging from BNB Chain requires BNB for Gas.
* Bridging from Arbitrum requires ETH for Gas.

### Step-by-Step Guide to Bridging Assets to X Layer

Official X Layer bridge entry:\
https://web3.okx.com/xlayer/bridge

#### Step 1: Open the OKX DEX Cross-Chain Bridge

Go to the official X Layer bridge page.

Enter the OKX DEX cross-chain bridge interface.

<img src="../.gitbook/assets/unknown (18).png" alt="" height="303" width="624">

#### Step 2: Select the Source Network, Destination Network, and Assets

#### 1. Set the “From” section

* Click the network icon at the top.
* Select the network where your assets are currently located, such as Ethereum.
* Click the token icon.
* Select the asset you want to bridge, such as USDT.

#### 2. Set the “To” section

* Click the destination network icon.
* Select X Layer as the destination network.
* Click the token icon.
* Select the asset you want to receive on X Layer, such as USDT or OKB.

<img src="../.gitbook/assets/unknown (19).png" alt="" height="283" width="624">

#### Step 3: Enter the Amount and Review the Recommended Route

Enter the amount you want to bridge in the “From” section.

The OKX DEX aggregator will automatically calculate and recommend a cross-chain route based on factors such as execution speed, slippage, and total cost.

Carefully review the information displayed on the page, including:

* Estimated amount received
* Source-network Gas fee
* Cross-chain bridge fee
* Estimated completion time
* Minimum amount received
* Cross-chain service provider or routing protocol

<div><img src="../.gitbook/assets/unknown (20).png" alt="" height="273" width="315"> <img src="../.gitbook/assets/unknown (21).png" alt="" height="326" width="301"></div>

#### Step 4: Approve the Token and Confirm the Transaction

After confirming that all information is correct, click the Cross-chain Swap button at the bottom of the page.

If this is your first time bridging the selected token, your wallet may ask you to approve the token.

Complete the approval transaction by following the wallet instructions.

After the approval is confirmed, review the transaction details again.

Confirm the transaction in your wallet and pay the Gas fee on the source network.

Please note that token approval and the actual cross-chain transaction may be two separate on-chain transactions, each requiring a Gas fee.

#### Step 5: Track the Transaction and Check Your Assets

After the transaction is submitted, you can check its progress in the transaction history section.

Cross-chain transfers usually take several minutes, depending on the confirmation speed of the source network and the selected bridge route.

Once the transaction is completed, return to your Web3 wallet.

Switch the wallet network to X Layer.

Check whether the bridged assets have arrived.

If the asset does not appear automatically, you may need to manually import the token contract into your wallet.

<img src="../.gitbook/assets/unknown (23).png" alt="" height="195" width="624">

### Important Details and Risk Warnings

Before interacting with X Layer, please carefully review the following information.

#### 1. Important: OKB Is the Native Gas Token of X Layer

X Layer uses OKB as its native Gas token.

This means that if you bridge only USDT, USDC, or another token to X Layer but do not have any OKB, you may be unable to transfer assets, swap tokens, approve contracts, or interact with decentralized applications on X Layer.

#### Recommended Solutions

**Option A: Withdraw OKB from OKX**

The simplest and generally most convenient method is to withdraw a small amount of OKB from your OKX exchange account to your Web3 wallet.

When withdrawing, make sure you select X Layer as the withdrawal network.

Always verify the receiving address and selected network before confirming the withdrawal.

**Option B: Use a Bridge Route That Supports Destination Gas**

Some third-party bridges or bridge aggregators may provide a destination Gas feature. This feature allows users to automatically convert a small portion of the bridged assets into the destination network’s native Gas token.

Availability depends on the selected route, token, network, and bridge provider. Always review the transaction details before signing.

\[Insert screenshot here: destination Gas or Gas-refuel option, if available]

#### 2. Bridging Time and Withdrawal Mechanisms

**Depositing Assets into X Layer**

Depositing assets into X Layer through the official bridge or a third-party bridge is generally fast. In most cases, funds may arrive within several minutes.

Actual completion time depends on:

* Source-network congestion
* Block confirmation requirements
* The selected cross-chain protocol
* Available bridge liquidity
* Security or risk-control checks

**Withdrawing Assets from X Layer**

The required withdrawal time may vary depending on the bridge route.

**Official Canonical Bridge**

When withdrawing assets from X Layer to Ethereum through the official canonical bridge, users may be required to wait through an Optimistic Rollup challenge period.

This waiting period may take approximately seven days.

**Third-Party Liquidity Bridges**

Third-party liquidity bridges, such as Stargate or Owlto, may allow users to transfer assets out of X Layer within several minutes.

These bridges use liquidity pools or market makers to provide assets on the destination network before the canonical settlement process is completed.

However, users may need to pay additional fees, including:

* Liquidity provider fees
* Bridge service fees
* Slippage
* Source-network and destination-network Gas fees

Before confirming a transaction, compare the estimated arrival time, total fees, minimum amount received, and bridge provider.

#### 3. Beware of Fake Websites and Phishing Attacks

Always access the bridge through the official OKX App or the official OKX Web3 domain:

https://web3.okx.com

Do not open bridge links sent by unknown accounts, private messages, unofficial advertisements, or unverified community members.

Before approving or signing a transaction:

* Check the website domain carefully.
* Confirm that your wallet is connected to the correct network.
* Review the token and amount being authorized.
* Check whether the approval is limited or unlimited.
* Verify the interacting smart contract whenever possible.
* Never enter your seed phrase or private key on any website.
* Reject unfamiliar signature requests.

For additional security, consider testing the bridge with a small amount before transferring a larger amount.

<br>
