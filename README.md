# LoopFi Bounty Details
- Until TVL < $500,000
  - Critical: $50,000
- Once TVL > $500,0000
  - Critical: $100,000
- High severity: $25,000 - $50,000
- Medium severity: $10,000 - $25,000

Join [C4 Discord](https://discord.gg/code4rena) to register

Submit findings [using the C4 form](https://code4rena.com/bounties/SponsorName/submit)

[Read our Code4rena Blue guidelines for more details](https://docs.google.com/document/d/1jzNh1Bat5iK6ryqvQ41_8GQjQ-ifxhHDlFINL_uijr4/edit?usp=sharing)

❗ _Note for participants: The sponsor's repo, scope definition, and contents herein are all subject to change._

## Publicly Known Issues

LoopFi commits to providing Known Issue Assurance to bug submissions through their program. This means that LoopFi will either disclose known issues publicly, or at the very least, privately via a self-reported bug submission. 

In a potential scenario of a mediation, this allows for a more objective and streamlined process, in order to prove that an issue is known. Otherwise, assuming the bug report is valid, it would result in the report being considered as in-scope, and due a reward.

Bug reports covering previously-discovered bugs (listed below) are not eligible for a reward within this program. This includes known issues that the project is aware of but has consciously decided not to “fix”, necessary code changes, or any implemented operational mitigating procedures that can lessen potential risk. 




# Project Overview

LoopFi is a dedicated lending market for Ethereum carry trades. Users can supply a long tail of 
Liquid Restaking Tokens (LRT) and their derivatives (e.g., Pendle LP tokens) as collateral to borrow 
ETH for increased yield and points exposure.

For more information about LoopFi, please visit https://www.loopfi.xyz/.


## Links

- **Previous audits:** [List of completed audits](https://docs.loopfi.xyz/extras/security)
- **Documentation:** [Loopfi Documentation](https://docs.loopfi.io/)
- **Codebase:** [Loopfi-contracts](https://github.com/loopfi-io/loopfi-contracts.) 
- **Website:** [Visit Website](https://www.loopfi.xyz/)
- **Twitter:** [Profile](https://x.com/loopfixyz)
- **Discord:** [Check LinkTree](https://tr.ee/31_WN-0wcv)


# Scope


| Contract | SLOC | Purpose | Libraries used |  
| ----------- | ----------- | ----------- | ----------- |
| [loop-prelaunch-contracts/blob/main/src/](https://github.com/LoopFi/loop-prelaunch-contracts/blob/main/src/PrelaunchPoints.sol) | 135 | Users can stake ETH into this contract, which will emit events tracked on a backed to calculate their corresponding amount of points. When staking, users can use a referral code encoded as bytes32 that will give the referral extra points. | [`@openzeppelin/*`](https://openzeppelin.com/contracts/) |
