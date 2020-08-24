## Summary

Trent Elmore, Brock Elmore, Will Price, Clinton Bembrey, and Dan Elitzer propose the following measures to be implemented for the launch of YAMv3 based on discussions with the YAM community over the past two weeks. Our motivation for submitting this proposal is to ensure an efficient transition from V2 to V3 that addresses mission-critical issues in the most fair way for the largest amount of the community possible. We believe this is the best path forward, but it is up to the community to decide, this is not an exhaustive list of possible changes, and we do expect additional proposals to be submitted.

As mentioned in the Proposal Mechanics proposal, anyone can submit further proposals which may supersede and/or iterate upon the below.

### Item 1: Minor Protocol Updates

We propose the following protocol updates. While there are many ideas on how the Yam protocol can be improved, we find it prudent to focus on minor updates that improve upon V1 with limited overhead.

Update reserve asset to yUSD (yyCRV), which has higher yield potential than yCRV
Replace YAMv1/yCRV sync() call on Uniswap V2 with YAMv3/yUSD sync() call
Hardcode proposal (50K pre-rebase) and quorum (200k pre-rebase) thresholds
Make voting period 2 days instead of 3 for quicker governance action
Complete audit of fully functional YAMv3 protocol

### Item 2: YAMv3 Incentivization Distribution

We propose a single farming pool be established on the YAMv3/yUSD (yyCRV) Uniswap V2 LP pool. The first week of incentives will begin one hour after V3 launch and total 330,000 YAMv3. Incentives will be reduced by 30% each week, resulting in a total of 1.1MM YAMv3 tokens distributed to stakers.

We also propose a 1MM YAMv3 community fund, held outside the reserve in a separate community fund contract. This fund will be controlled by V3 governance, will not impact quorum requirements for voting, and can be used as the community sees fit. Uses may include but are not limited to new incentivized pools or ecosystem development initiatives.

TL;DR:
YAM/yUSD LP Incentivized  Staking Pool, initial weekly issuance of 330k YAMv3, decreasing 30% each week, totalling 1.1MM.
1MM YAMv3 Community Fund

### Item 3: YAMv2 to YAMv3 Migration

We propose a 1:1 migration for YAMv2 holders. A migration contract with no deadline will be created, which will allow YAMv2 holders to burn their YAMv2 tokens in exchange for YAMv3 tokens.

TL;DR:
1:1 migration from V2 to V3 via migration contract

### Item 4: Delegator Rewards

We propose utilizing a snapshot taken at the time of the #saveyam governance proposal to reward delegators utilizing a “flat and scaled” reward model. The list of delegators can be found here: https://raw.githubusercontent.com/yam-finance/yam-protocol/master/yam_delegator_snapshot_10650187_draft.json

The rewards will also be used to bring the total supply of YAMv3 to a round number, by the following calculation:

 (YAMv3 Total Supply) - (Community Fund) - (LP Pool Incentives) -  (YAMv2 Total Supply) = (Delegator Rewards)

Total delegator rewards will be approximately 173,588.383 YAMv3. We propose to distribute half (approximately 86,794.192) of these rewards on a flat basis to the 3,173 delegators, rewarding each delegate with approximately 27.354 YAMv3 tokens. The remaining 86,794.192 YAMv3 tokens will be distributed to delegators in proportion to their percentage of total votes delegated. This structure compensates small holders for their efforts and incurred transaction fees, as well as compensating all holders for their proportional impact.

These delegator rewards will be fully vested on V3 launch.

TL;DR:
Approximately 173k in rewards, half distributed on flat scale to all delegators, half distributed proportional to voting contribution

### Proposal Summary:

Total V3 Supply: 6,000,000

Protocol Updates:
Update reserve asset to yUSD (yyCRV), which has higher yield potential than yCRV.
Call sync() on Uniswap V2 YAMv3/yUSD pool
Hardcode proposal (50K) and quorum (200k) thresholds
Make voting period 2 days instead of 3
Complete audit of fully functional YAMv3 protocol

Farming and Incentives:
YAM/yUSD LP Pool, receiving 330k YAMv3, decreasing 30% each week, totalling 1.1M.
1M YAMv3 Community Fund

Migration:
1:1 migration from V2 to V3

Delegator Rewards:
Approximately 173k in rewards, half distributed equally to all delegators, half distributed according to a linear scale of voting contribution

Once again, this proposal is made by the individuals who originally launched YAM, and reflects our thoughts on how to best proceed. Ultimately, it is up to the community of YAM to decide, and proposals meeting the minimum requirements may supersede or iterate upon this proposal.
