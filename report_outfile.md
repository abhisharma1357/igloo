## Sūrya's Description Report

### Files Description Table


|  File Name  |  SHA-1 Hash  |
|-------------|--------------|
| IglooMasterV7.22+Strategies.sol | 02b91d5509c40da3ae20555a8243407a8ddab82b |


### Contracts Description Table


|  Contract  |         Type        |       Bases      |                  |                 |
|:----------:|:-------------------:|:----------------:|:----------------:|:---------------:|
|     └      |  **Function Name**  |  **Visibility**  |  **Mutability**  |  **Modifiers**  |
||||||
| **IERC20** | Interface |  |||
| └ | totalSupply | External ❗️ |   |NO❗️ |
| └ | balanceOf | External ❗️ |   |NO❗️ |
| └ | transfer | External ❗️ | 🛑  |NO❗️ |
| └ | allowance | External ❗️ |   |NO❗️ |
| └ | approve | External ❗️ | 🛑  |NO❗️ |
| └ | transferFrom | External ❗️ | 🛑  |NO❗️ |
||||||
| **PEFI** | Interface | IERC20 |||
| └ | mint | External ❗️ | 🛑  |NO❗️ |
| └ | setMinter | External ❗️ | 🛑  |NO❗️ |
||||||
| **PenguinNests** | Interface | IERC20 |||
| └ | enter | External ❗️ | 🛑  |NO❗️ |
| └ | currentExchangeRate | External ❗️ |   |NO❗️ |
||||||
| **IRewarder** | Interface |  |||
| └ | onPefiReward | External ❗️ | 🛑  |NO❗️ |
| └ | pendingTokens | External ❗️ |   |NO❗️ |
||||||
| **IIglooStrategy** | Interface |  |||
| └ | deposit | External ❗️ | 🛑  |NO❗️ |
| └ | withdraw | External ❗️ | 🛑  |NO❗️ |
| └ | inCaseTokensGetStuck | External ❗️ | 🛑  |NO❗️ |
| └ | setAllowances | External ❗️ | 🛑  |NO❗️ |
| └ | revokeAllowance | External ❗️ | 🛑  |NO❗️ |
| └ | migrate | External ❗️ | 🛑  |NO❗️ |
| └ | onMigration | External ❗️ | 🛑  |NO❗️ |
| └ | pendingTokens | External ❗️ |   |NO❗️ |
| └ | transferOwnership | External ❗️ | 🛑  |NO❗️ |
||||||
| **IStakingRewards** | Interface |  |||
| └ | totalSupply | External ❗️ |   |NO❗️ |
| └ | balanceOf | External ❗️ |   |NO❗️ |
| └ | lastTimeRewardApplicable | External ❗️ |   |NO❗️ |
| └ | rewardPerToken | External ❗️ |   |NO❗️ |
| └ | earned | External ❗️ |   |NO❗️ |
| └ | getRewardForDuration | External ❗️ |   |NO❗️ |
| └ | stake | External ❗️ | 🛑  |NO❗️ |
| └ | stakeWithPermit | External ❗️ | 🛑  |NO❗️ |
| └ | withdraw | External ❗️ | 🛑  |NO❗️ |
| └ | getReward | External ❗️ | 🛑  |NO❗️ |
| └ | exit | External ❗️ | 🛑  |NO❗️ |
||||||
| **Address** | Library |  |||
| └ | isContract | Internal 🔒 |   | |
| └ | sendValue | Internal 🔒 | 🛑  | |
| └ | functionCall | Internal 🔒 | 🛑  | |
| └ | functionCall | Internal 🔒 | 🛑  | |
| └ | functionCallWithValue | Internal 🔒 | 🛑  | |
| └ | functionCallWithValue | Internal 🔒 | 🛑  | |
| └ | functionStaticCall | Internal 🔒 |   | |
| └ | functionStaticCall | Internal 🔒 |   | |
| └ | functionDelegateCall | Internal 🔒 | 🛑  | |
| └ | functionDelegateCall | Internal 🔒 | 🛑  | |
| └ | verifyCallResult | Internal 🔒 |   | |
||||||
| **SafeERC20** | Library |  |||
| └ | safeTransfer | Internal 🔒 | 🛑  | |
| └ | safeTransferFrom | Internal 🔒 | 🛑  | |
| └ | safeApprove | Internal 🔒 | 🛑  | |
| └ | safeIncreaseAllowance | Internal 🔒 | 🛑  | |
| └ | safeDecreaseAllowance | Internal 🔒 | 🛑  | |
| └ | _callOptionalReturn | Private 🔐 | 🛑  | |
||||||
| **Ownable** | Implementation |  |||
| └ | <Constructor> | Public ❗️ | 🛑  |NO❗️ |
| └ | owner | Public ❗️ |   |NO❗️ |
| └ | renounceOwnership | Public ❗️ | 🛑  | onlyOwner |
| └ | transferOwnership | Public ❗️ | 🛑  | onlyOwner |
||||||
| **IglooStrategyBase** | Implementation | IIglooStrategy, Ownable |||
| └ | <Constructor> | Public ❗️ | 🛑  |NO❗️ |
| └ | pendingTokens | External ❗️ |   |NO❗️ |
| └ | deposit | External ❗️ | 🛑  | onlyOwner |
| └ | withdraw | External ❗️ | 🛑  | onlyOwner |
| └ | inCaseTokensGetStuck | External ❗️ | 🛑  | onlyOwner |
| └ | setAllowances | External ❗️ | 🛑  | onlyOwner |
| └ | revokeAllowance | External ❗️ | 🛑  | onlyOwner |
| └ | migrate | External ❗️ | 🛑  | onlyOwner |
| └ | onMigration | External ❗️ | 🛑  | onlyOwner |
| └ | transferOwnership | Public ❗️ | 🛑  | onlyOwner |
||||||
| **IglooStrategyStorage** | Implementation | Ownable |||
| └ | increaseRewardDebt | External ❗️ | 🛑  | onlyOwner |
| └ | decreaseRewardDebt | External ❗️ | 🛑  | onlyOwner |
| └ | setRewardDebt | External ❗️ | 🛑  | onlyOwner |
| └ | increaseRewardTokensPerShare | External ❗️ | 🛑  | onlyOwner |
||||||
| **IglooStrategyForPangolinStaking** | Implementation | IglooStrategyBase |||
| └ | <Constructor> | Public ❗️ | 🛑  | IglooStrategyBase |
| └ | checkReward | Public ❗️ |   |NO❗️ |
| └ | pendingRewards | Public ❗️ |   |NO❗️ |
| └ | rewardTokens | External ❗️ |   |NO❗️ |
| └ | pendingTokens | External ❗️ |   |NO❗️ |
| └ | harvest | External ❗️ | 🛑  |NO❗️ |
| └ | deposit | External ❗️ | 🛑  | onlyOwner |
| └ | withdraw | External ❗️ | 🛑  | onlyOwner |
| └ | migrate | External ❗️ | 🛑  | onlyOwner |
| └ | onMigration | External ❗️ | 🛑  | onlyOwner |
| └ | setAllowances | External ❗️ | 🛑  | onlyOwner |
| └ | _claimRewards | Internal 🔒 | 🛑  | |
| └ | _harvest | Internal 🔒 | 🛑  | |
| └ | _safeRewardTokenTransfer | Internal 🔒 | 🛑  | |
||||||
| **IglooMaster** | Implementation | Ownable |||
| └ | <Constructor> | Public ❗️ | 🛑  |NO❗️ |
| └ | poolLength | Public ❗️ |   |NO❗️ |
| └ | totalPendingPEFI | Public ❗️ |   |NO❗️ |
| └ | pendingPEFI | Public ❗️ |   |NO❗️ |
| └ | pendingIPEFI | Public ❗️ |   |NO❗️ |
| └ | pendingRewards | Public ❗️ |   |NO❗️ |
| └ | pendingTokens | External ❗️ |   |NO❗️ |
| └ | reward | Public ❗️ |   |NO❗️ |
| └ | pefiPerYear | Public ❗️ |   |NO❗️ |
| └ | pefiPerYearToIgloo | Public ❗️ |   |NO❗️ |
| └ | pefiPerYearToNest | Public ❗️ |   |NO❗️ |
| └ | nestAPY | Public ❗️ |   |NO❗️ |
| └ | totalShares | Public ❗️ |   |NO❗️ |
| └ | totalLP | Public ❗️ |   |NO❗️ |
| └ | userShares | Public ❗️ |   |NO❗️ |
| └ | profitInLP | Public ❗️ |   |NO❗️ |
| └ | ipefiDistributionBipsByUser | Public ❗️ |   |NO❗️ |
| └ | updatePool | Public ❗️ | 🛑  |NO❗️ |
| └ | massUpdatePools | Public ❗️ | 🛑  |NO❗️ |
| └ | deposit | External ❗️ | 🛑  | onlyApprovedContractOrEOA |
| └ | withdraw | External ❗️ | 🛑  | onlyApprovedContractOrEOA |
| └ | harvest | External ❗️ | 🛑  | onlyApprovedContractOrEOA |
| └ | withdrawAndHarvest | External ❗️ | 🛑  | onlyApprovedContractOrEOA |
| └ | emergencyWithdraw | External ❗️ | 🛑  | onlyApprovedContractOrEOA |
| └ | setIpefiDistributionBips | External ❗️ | 🛑  |NO❗️ |
| └ | add | External ❗️ | 🛑  | onlyOwner |
| └ | set | External ❗️ | 🛑  | onlyOwner |
| └ | migrateStrategy | External ❗️ | 🛑  | onlyOwner |
| └ | setStrategy | External ❗️ | 🛑  | onlyOwner |
| └ | manualMint | External ❗️ | 🛑  | onlyOwner |
| └ | transferMinter | External ❗️ | 🛑  | onlyOwner |
| └ | setDev | External ❗️ | 🛑  | onlyOwner |
| └ | setNest | External ❗️ | 🛑  | onlyOwner |
| └ | setNestAllocatorAddress | External ❗️ | 🛑  | onlyOwner |
| └ | setDevMintBips | External ❗️ | 🛑  | onlyOwner |
| └ | setNestMintBips | External ❗️ | 🛑  | onlyOwner |
| └ | setNestSplitBips | External ❗️ | 🛑  | onlyOwner |
| └ | setPefiEmission | External ❗️ | 🛑  | onlyOwner |
| └ | setDefaultIpefiDistributionBips | External ❗️ | 🛑  | onlyOwner |
| └ | modifyApprovedContracts | External ❗️ | 🛑  | onlyOwner |
| └ | setOnlyApprovedContractOrEOAStatus | External ❗️ | 🛑  | onlyOwner |
| └ | inCaseTokensGetStuck | External ❗️ | 🛑  | onlyOwner |
| └ | setAllowances | External ❗️ | 🛑  | onlyOwner |
| └ | revokeAllowance | External ❗️ | 🛑  | onlyOwner |
| └ | accountAddedLP | External ❗️ | 🛑  |NO❗️ |
| └ | safePEFITransfer | Internal 🔒 | 🛑  | |


### Legend

|  Symbol  |  Meaning  |
|:--------:|-----------|
|    🛑    | Function can modify state |
|    💵    | Function is payable |
