# Ethereum based ERC20 compliant token
 An ERC20 compliant Token &amp; Crowdsale Application on Ethereum Platform written in truffle framework.




# Status Network Token
[![Build Status](https://travis-ci.org/status-im/status-network-token.svg?branch=master)](https://travis-ci.org/status-im/status-network-token)

- [Whitepaper](https://chronologic.network/uploads/Chronologic_Whitepaper.pdf)
- [The Big Picture: TimeMints, ChronoPower & Proof-of-Time](https://blog.chronologic.network/the-big-picture-timemints-chronopower-proof-of-time-f881158b044d) blogpost.


## Technical definition

At the technical level SGT & SNT are a ERC20-compliant tokens, derived from the [MiniMe Token](https://github.com/Giveth/minime) that allows for token cloning (forking), which will be useful for many future use-cases.

Also built in the token is a vesting schedule for limiting SNT transferability over time. Status Project Founders tokens are vesting.

## Contracts

- [AddressCappedCrowdsale.sol](/contracts/AddressCappedCrowdsale.sol): Child contract of Crowdsale.sol, making it address capped
- [BonusFinalizeAgent.sol](/contracts/BonusFinalizeAgent.sol): Child contract of FinalizeAgent.sol. Used to finalize crowdsale
- [ConsenSysWallet.sol](/contracts/ConsenSysWallet.sol): ConsenSys Multi Signature wallet Contract
- [Crowdsale.sol](/contracts/Crowdsale.sol): Main Crowdsale contract.
- [DayToken.sol](/contracts/DayToken.sol): Main contract for the Day Token
- [ERC20.sol](/contracts/ERC20.sol): Standard ERC20 token code
- [ERC20Basic.sol](/contracts/ERC20Basic.sol): Standard ERC20 Basic token code
- [FinalizeAgent.sol](/contracts/FinalizeAgent.sol): Contract code used to finalise crowdsale
- [FlatPricing.sol](/contracts/FlatPricing.sol): Contract to define pricing of DayTokens during Crowdsale
- [Haltable.sol](/contracts/Haltable.sol): Standard Haltable ERC20 token code
- [MintableToken.sol](/contracts/MintableToken.sol): Adds Minting feature to DayToken
- [Ownable.sol](/contracts/Ownable.sol): Standard ERC20 token code for ownership of DayToken
- [PricingStrategy.sol](/contracts/PricingStrategy.sol): Contract responsible for defining the pricing statergy of DayToken during Crowdsale
- [ReleasableToken.sol](/contracts/ReleasableToken.sol): Standard ERC20 token code making the token Releasable
- [SafeMathLib.sol](/contracts/SafeMathLib.sol): Contract responsible for executing all math operations safely
- [StandardToken.sol](/contracts/StandardToken.sol): Standard ERC20 token code
- [UpgradeAgent.sol](/contracts/UpgradeAgent.sol): Defines UpgradeAgent, letting owner upgrade the token code
- [UpgradeableToken.sol](/contracts/UpgradeableToken.sol): Standard ERC20 token code making the token Upgradeable
- [newToken.sol](/contracts/newToken.sol): New code for the upgraded token

See [INSTRUCTIONS.md](/INSTRUCTIONS.md) for instructions on how to test and deploy the contracts.

## Reviewers and audits.

Code for the Day token is being reviewed by:
