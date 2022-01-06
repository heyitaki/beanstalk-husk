# Beanstalk Pod Fungibility Proposal

## Introduction

Note: This proposal will likely not be implemented in its current form because the Pod pricing function doesn't take into external factors such as trust in the protocol (which may be measured by number of Harvested Pods). There may be an elegant solution applying this thinking to the Pod marketplace already in the works where we use each sale to price the Plots involved and extrapolate the Pods' future prices with the same exponential relationship explored in the proposal.

Pods are inherently non-fungible, but unlike most NFTs, the only difference between Pods is their positions in the Field queue. This proposal aims to introduce a method to price Pods and therefore allow a fungible representation of Pods that can then be used to create a liquidity pool to provide immediate and consistent liquidity for the Pod market.

## To-do

The current proposal needs to address two issues:

1. Exchanging a Pod for Husks does not reflect the future value of the Pod in the user's Husk balance. This may be solved with a yield generation scheme that allows users to stake their Plots to accrue Husks correlating to the increase in value of the Pod as calculated by the pricing function.

2. Equation 3 in the proposal actually introduces an inequality, not a strict equality. Traders are able to arbitrage the price of a Pod at the end of the queue if it increases above the limit set in Equation 3 by Sowing new Pods and selling them immediately, but there is no arbitrage opportunity in the reverse direction. Therefore, as discussed in the introduction, external factors such as probability of the protocol's future success may cause the Pod to trade at a price lower than it takes to Sow.

## Acknowledgements
Thanks to [Evan](https://twitter.com/EvanDeKim), [Ken](https://twitter.com/kenadia), [Julia](https://twitter.com/thejuliawu), [Sam](https://twitter.com/samclearman), [Cat](https://twitter.com/0xcatwu), and [Emma](https://twitter.com/emmaytang) for helping come up with the ideas presented in this proposal, and of course to the Beanstalk community.
