# WireGuard Implementation for the Zephyr Project

This project is a C implementation of the [WireGuard&reg;](https://www.wireguard.com/) protocol intended to be used within the [Zephyr Project&reg;](https://zephyrproject.org/) environment. A large majority of the codebase will be borrowed from the [WireGuard LwIP project](https://github.com/smartalock/wireguard-lwip) due to the platform-agnostic nature and the focus on integration with generic network stacks, making it adaptable to various environments, including Zephyr, which supports lwIP.

# Motivation

The core issue of security for IoT devices is the extreme lack of standardization in the Operating Systems and frameworks provided by the manufacturer of the respective device. The Zephyr Project aims to solve this, and is designed to run on extremely resource constrained IoT devices.

The main reason for implementing WireGuard on such devices is to isolate each device on its own Virtual LAN running on WireGuard, due to the protocol's nature, that being its small footprint while conserving relatively high performance.

Implementing WireGuard to run within Zephyr RTOS hence allows all boards supported by the project to use the protocol for the reasons stated earlier.

# More Information

WireGuard&reg; was created and developed by Jason A. Donenfeld. "WireGuard" and the "WireGuard" logo are registered trademarks of Jason A. Donenfeld. See https://www.wireguard.com/ for more information

This project is not approved, sponsored or affiliated with WireGuard or with the community.

- The whitepaper https://www.wireguard.com/papers/wireguard.pdf
- The Wikipedia page https://en.wikipedia.org/wiki/WireGuard 

# License

THis project is a fork of the [WireGuard LwIP project](https://github.com/smartalock/wireguard-lwip) and will hence retain the same license.

The code is copyrighted under BSD 3 clause Copyright (c) 2021 Daniel Hope (www.floorsense.nz)

See LICENSE for details
