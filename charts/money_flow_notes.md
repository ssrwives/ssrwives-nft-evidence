# Where the NFT money went

Prepared October 23, 2026 from preserved Ethereum records. Main chart: March 21–July 31, 2023 UTC. Payroll follow-through: May 12, 2023–March 8, 2024 UTC. The last payout occurred March 7 in Pacific time.

SSRWives raised **147.16 ETH**, approximately **$267,004** at the daily prices when the mint payments arrived. The collection issued 3,210 NFTs: 2,880 paid and 330 free or reserve tokens. The amount raised excludes 30 reverted candidate transactions.

The contract sent 125.626666666666666668 ETH to its deployer wallet and 10.766666666666666666 ETH each to its hard-coded `kyokoWallet` and `artWallet`. All 147.16 ETH had been withdrawn by May 12, 2023 UTC. The 30 internal transfers came from 12 withdrawal transactions.

The two publicly attributed founder wallets received **61.173333333333333332 ETH** from the mint contract and deployer through July 2023—approximately **$111,149** at the dates of those transfers. `kyokoWallet`, associated publicly with bbykyoko.eth, received 31.136666666666666666 ETH. `artWallet`, associated publicly with hedprotag, received 30.036666666666666666 ETH.

The named payroll wallet received **56.01 ETH**, approximately **$101,286** at transfer. A Coinbase-labelled deposit address received **32.21 ETH**, approximately **$58,573**. Its exchange account holder is unidentified. The 19 ETH transfer on May 12 is already included in the 32.21 ETH cumulative amount.

The deployer also received **3.031953645999154159 ETH from other sources**. These extra receipts appear as their own input in the chart. The downstream totals are gross wallet flows; no percentage is represented as an exclusive slice of the mint.

The payroll wallet swapped **53 ETH for 93,086.200052 USDC**, then made **39 payouts totalling 92,962.114971 USDC to seven addresses**. Those payouts included **5,500.114971 USDC to kyokoWallet**. Its final USDC payout, 1,500.114971 USDC, went to kyokoWallet on March 8, 2024 UTC. The resulting balances were **0 USDC and 0.00036369216618 ETH**. The payroll panel is a later stage of the 56.01 ETH already shown in the Sankey.

## Exact reconciliation

| Deployer inflows | ETH |
|---|---:|
| From mint contract | 125.626666666666666668 |
| Other normal transfers | 2.389801590510488699 |
| Other internal transfers | 0.642152055488665460 |
| **Total in** | **128.658620312665820827** |

| Deployer outflows and balance | ETH |
|---|---:|
| Named payroll wallet | 56.01 |
| Coinbase-labelled deposit | 32.21 |
| kyokoWallet | 20.37 |
| artWallet | 19.27 |
| Other addresses | 0.55 |
| Transaction gas | 0.173210523279100870 |
| Derived closing balance, July 31, 2023 | 0.075409789386719957 |
| **Total out and remaining** | **128.658620312665820827** |

The complete chart conserves 150.191953645999154159 ETH: the 147.16 ETH mint plus 3.031953645999154159 ETH in other deployer receipts. That is equal to the destination totals, deployer gas and deployer closing balance.

The payroll USDC ledger reconciles exactly: 93,086.200052 received − 92,962.114971 payouts − 120 swap-spender transfer − 4.085081 net round-trip difference = 0 USDC. The authentic USDC contract is `0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48`; lookalike token spam is excluded. Self-transfers net to zero. Every tabulated token amount was matched to its preserved original authentic-USDC transaction log.

The payroll ETH ledger also reconciles: 56.01 external receipts + 0.071759261881557627 swap return − 55.978161719713559265 sent (including the 53 ETH swap) − 0.103233850001818362 gas = 0.00036369216618 ETH. This equals the preserved balance record.

## Evidence and labels

- **E04:** [Verified NFT contract](https://etherscan.io/address/0x64256b6409150e8b2b25a456a17dcf171209542a#code), preserved wallet histories, mint ledger and receipts, authentic USDC logs, and daily ETH/USD price records. Contract code supplies the `kyokoWallet` / `artWallet` names. Preserved OpenSea profiles supply the public bbykyoko.eth / hedprotag attributions.
- **E05:** [Official treasury and salary disclosure](https://x.com/ssrwives/status/1656847125236334593), May 12, 2023 UTC: half of the remaining treasury for future-developer payroll, the other half as advance team salaries. [The 56 ETH payroll transfer](https://etherscan.io/tx/0xe0a46b49cb7b2c5c2294e5d508cef543f2cf5e8dd7f18c6510bb4780951ccf58) followed the small 0.01 ETH transfer.
- [Earlier allocation statement](https://x.com/ssrwives/status/1653504925970714643), May 2, 2023: two-thirds of mint money described as going directly to game development. The amount at one labelled payroll address is a distinct measure from total project development expenses.
- [53 ETH → USDC swap](https://etherscan.io/tx/0x99bec7faf9c4f56ab53e59afe26dbb46ba2dfac408e841e55583fc351173b19c), May 12, 2023 UTC.
- [Final 1,500.114971 USDC payout to kyokoWallet](https://etherscan.io/tx/0x0081641448300d07e85bf3f9e830e7536054f90ba03388504b91af7bd568560f), March 8, 2024 UTC.

Original records are supplied under `../evidence/E04/`, including price records in its `prices/` folder. Their fingerprints and archive paths are in `../SOURCE_MANIFEST.json`. `money_flow_data.json` supplies every chart edge, exact amounts and transaction links. The tables reconcile the preserved transfers, fees and balances.

Dollar labels use the Coinbase Exchange closing ETH/USD price for each transaction's UTC day. Mint dollars are valued at receipt; subsequent dollars are valued at transfer. They are historical approximations. The ETH scale is conserved; USD totals across hops can differ because dates and prices differ. USDC is shown at face value.
