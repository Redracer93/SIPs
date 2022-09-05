---
sccp: 227
network: Ethereum
title: Increase Atomic Twap Window - Atomic Swaps
author: Kaleb (@kaleb-keny)
status: Vote_Pending
proposal: >-
  https://snapshot.org/#/snxgov.eth/proposal/0xbde0a36eff2e658c0dc1f84047d426629e2b68fdea063a0f2daab19fb7c1fcd4
created: 2022-09-05
type: Governance
---

## Simple Summary

<!--"If you can't explain it simply, you don't understand it well enough." Provide a simplified and layman-accessible explanation of the SCCP.-->

This SCCP proposes to increase atomic twap window to 30 minutes from 1 minute.


## Abstract

<!--A short (~200 word) description of the variable change proposed.-->

The `atomicTwapWindow` is the twap window used when fetching the uniswap price.

## Motivation

<!--The motivation is critical for SCCPs that want to update variables within Synthetix. It should clearly explain why the existing variable is not incentive aligned. SCCP submissions without sufficient motivation may be rejected outright.-->

The atomic twap window was originally lowered to 1 minute due to a bug in the atomic exchange function that has been long patched with [SIP-258](https://sips.synthetix.io/sips/sip-258/). In order to improve security on the exchange function, as well as lower the chance of latency arbitrage, this SCCP proposes to increase the TWAP window back to 30 minutes.

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).