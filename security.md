---
description: This page documents the various audits taken to secure the protocol
---

# Security

SomeETHing is built with security as a fundamental principle, implementing multiple layers of protection to ensure the safety of tokens and users. The platform's security architecture is designed to be resilient against various attack vectors while maintaining full functionality.

SomeETHing is open source and the source code for the underlying contracts can be found in our GitHub.

{% @github-files/github-code-block url="https://github.com/SomETHingdotfun/contracts/" %}

## GoPlus Locker Integration

Every token launched through SomeETHing is automatically locked using GoPlus Locker, providing several security benefits:

- **Automatic Locking**: Tokens are locked immediately upon launch
- **Fee Structure**: 2.8% of trading fees support the locker service
- **Continuous Protection**: Locks remain active throughout the token's lifecycle
- **Transparent Verification**: Lock status is publicly verifiable

Learn more about GoPlus and liquidity locking by visiting the [GoPlus Docs](https://docs.gopluslabs.io/page/goplus-safetoken-locker)

## Token Implementation

All SomeETHing tokens follow a secure, minimal implementation approach:

- **Simple Contract Design**: Reduced attack surface through minimal code
- **Ownership Renouncement**: Token ownership is automatically renounced after launch
- **No Hidden Functions**: Transparent, auditable token code
- **Standard Compliance**: Implements widely-tested ERC20 standards

{% @github-files/github-code-block url="https://github.com/SomETHingdotfun/contracts/blob/main/contracts/SomeToken.sol" %}

## Deployment Addresses & Ownership

All deployments are protected via timelocks and multisigs.

- **Timelock Address (Linea)**: `----`
- **ProxyAdmin**: `----`
- **Gnosis Safe**: `----`
