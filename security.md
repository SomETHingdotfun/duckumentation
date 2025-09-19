---
description: This page documents the various audits taken to secure the protocol
---

# Security

SOMETHING is built with security as a fundamental principle, implementing multiple layers of protection to ensure the safety of tokens and users. The platform's security architecture is designed to be resilient against various attack vectors while maintaining full functionality.

SOMETHING is open source and the source code for the underlying contracts can be found in our GitHub.

{% embed url="https://github.com/SomETHingdotfun/contracts/" %}

## GoPlus Locker Integration

Every token launched through SOMETHING is automatically locked using GoPlus Locker, providing several security benefits:

* **Automatic Locking**: Tokens are locked immediately upon launch
* **Fee Structure**: 2.8% of trading fees support the locker service
* **Continuous Protection**: Locks remain active throughout the token's lifecycle
* **Transparent Verification**: Lock status is publicly verifiable

Learn more about GoPlus and liquidity locking by visiting the [GoPlus Docs](https://docs.gopluslabs.io/page/goplus-safetoken-locker)

## Token Implementation

All SOMETHING tokens follow a secure, minimal implementation approach:

* **Simple Contract Design**: Reduced attack surface through minimal code
* **Ownership Renouncement**: Token ownership is automatically renounced after launch
* **No Hidden Functions**: Transparent, auditable token code
* **Standard Compliance**: Implements widely-tested ERC20 standards

{% @github-files/github-code-block url="https://github.com/SomETHingdotfun/contracts/blob/main/contracts/SomeToken.sol" %}

## Deployment Addresses & Ownership

All deployments are protected via timelocks and multisigs.

* **Timelock Address (Linea)**: [`0xc66E5424a8A1C5905574D7a23Dcb2387226C75b5`](https://lineascan.build/address/0xc66E5424a8A1C5905574D7a23Dcb2387226C75b5#code)
* **ProxyAdmin**: [`0x0FB4DD0bF5F7AE6Ca1e24Bb84ff7FE4B6190528A`](https://lineascan.build/address/0x0FB4DD0bF5F7AE6Ca1e24Bb84ff7FE4B6190528A)
* **Gnosis Safe**: `----`
