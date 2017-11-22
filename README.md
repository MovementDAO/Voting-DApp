# The Movement DAO Voting DApp

The Movement DAO is entirely owned and shaped by its participants. Without any central leader and built from the ground up, it supports humans on the internet to come together and create freely.

The MVT (Movement Token) allows participants to vote on the governance of the organization, thereby collectively shaping its presence and future. Votes are tied to specific proposals.


# The Vision

It is The Movement's vision to connect humans across borders and cultures, allowing people from all around the world to connect and create. The Movement is based on blockchain technology and builds a virtual reality headquarter to supply common ground and place, and to foster decentralized collaboration.


# Voting DApp Basic Functionality

The Movement Voting DApp allows MVT token holders to propose and vote. In the future The Movement will transition to [Aragon Core](https://github.com/aragon/aragon-core), putting into practice the next generation of decentralized governance. This version of the Voting DApp is forked from the [Gilgamesh Vote DApp](https://github.com/skiral/gilgamesh-vote-dapp) of the Gilgamesh Platform.


# How to Submit a Proposal?

In order to submit a proposal a new Github issue has to be posted on The Movement's Github repository (MovementDAO/DAO-Proposals). Proposals are reviewed and accepted by the community.


# The Movement Proposal Standard

All proposals should adhere to The Movement's standard proposal structure. 

**Name**: Include the name of your proposed idea/feature/sphere/development in both the first line of text and the title of the issue in our repository.

**Idea**: Explain your proposal. What are your ideas and visions? Try to be as detailed as possible.

**Summary**: Write one sentence that summarizes your proposal.

**ETH address**: Your personal ETH address




# Proposal Review and Approval

The Movement community discusses and reviews all proposals submitted via Github and asseses them for compliance with The Movement's Proposal Standard. After review, proposals are labeled [as follows](https://github.com/MovementDAO/DAO-Proposals/labels):

**Green** ("Approved"): The proposal followed all requirements and has been accepted for voting.

**Yellow** ("Pending"):  The proposal requires more content or some degree of revision to adhere to The Movement's Proposal Standard.

**Red** ("Denied"): This proposal has been denied.


# Voting and Unvoting

MVT token holders and the community of The Movement DAO participants can vote on approved submissions using one of the following two methods:

* Vote using the MetaMask Chrome extension developed by metamask.io. Fund your MetaMask account with MVT. Via The Movement's Voting Interface, click "Vote" on the proposal you want to vote for, and confirm the transaction via MetaMask.

* Vote using MyEtherWallet. Go to https://www.myetherwallet.com/#contracts. In the **"Contract Address"** field, insert The Movement Voting smart contract address: `0xee566744d093343a1c3211ae75402c33572a598d`.
Enter the following in the ABI/JSON Interface field:
```
[{"constant":true,"inputs":[],"name":"endBlock","outputs":[{"name":"","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":false,"inputs":[],"name":"unVote","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[{"name":"proposalId","type":"int256"}],"name":"vote","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":false,"inputs":[{"name":"_endBlock","type":"uint256"}],"name":"changeEndBlock","outputs":[],"payable":false,"stateMutability":"nonpayable","type":"function"},{"constant":true,"inputs":[{"name":"offset","type":"uint256"},{"name":"limit","type":"uint256"}],"name":"getVoters","outputs":[{"name":"_voters","type":"address[]"},{"name":"_proposalIds","type":"int256[]"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":true,"inputs":[],"name":"votersCount","outputs":[{"name":"","type":"uint256"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":true,"inputs":[{"name":"","type":"address"}],"name":"votes","outputs":[{"name":"","type":"int256"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":true,"inputs":[{"name":"","type":"uint256"}],"name":"voters","outputs":[{"name":"","type":"address"}],"payable":false,"stateMutability":"view","type":"function"},{"constant":true,"inputs":[],"name":"admin","outputs":[{"name":"","type":"address"}],"payable":false,"stateMutability":"view","type":"function"},{"inputs":[{"name":"_endBlock","type":"uint256"}],"payable":false,"stateMutability":"nonpayable","type":"constructor"},{"anonymous":false,"inputs":[{"indexed":true,"name":"voter","type":"address"},{"indexed":true,"name":"proposalId","type":"int256"}],"name":"onVote","type":"event"},{"anonymous":false,"inputs":[{"indexed":true,"name":"voter","type":"address"},{"indexed":true,"name":"proposalId","type":"int256"}],"name":"onUnVote","type":"event"}]
```
Press `Access` then select function `vote` or `unvote.` Insert the number from the GitHub issue ID of the selected proposal in the `proposalId` field. Send and sign the transaction. **Do NOT send any ETH, MVT, or any other token.**


# Proposal Incentives

To incentivize the submission of high quality and thoughtful contributions, The Movement DAO offers a Bounty Program. Learn more about the Bounty Program here: https://bitcointalk.org/index.php?topic=2068554.1560
