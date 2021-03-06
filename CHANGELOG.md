# Changelog

All notable changes to this project will be documented in this file.

## [v1.2.1](https://github.com/ValentinBELYN/icmplib/releases/tag/v1.2.1) - 2020-09-26
- Fix an issue in the `traceroute` function which gave the wrong value for the `avg_rtt` property (@patrickfnielsen).
- Some other tweaks to the `traceroute` function.

## [v1.2.0](https://github.com/ValentinBELYN/icmplib/releases/tag/v1.2.0) - 2020-09-12
- Add the ability to modify the traffic class of ICMP packets.
- Add new optional parameters to the `traceroute` function.
- Add a new exception `SocketUnavailableError` when an action is performed while a socket is closed.
- Add a warning message on deprecated properties.
- Explicit closure of sockets on built-in functions.
- Fix a bug when ICMP responses are not correctly formatted (part 2).

## [v1.1.3](https://github.com/ValentinBELYN/icmplib/releases/tag/v1.1.3) - 2020-09-03
- Fix a bug when ICMP responses are not correctly formatted.

## [v1.1.2](https://github.com/ValentinBELYN/icmplib/releases/tag/v1.1.2) - 2020-08-29
- Fix a compatibility issue.

## [v1.1.1](https://github.com/ValentinBELYN/icmplib/releases/tag/v1.1.1) - 2020-07-10
- Fix a bug when the source host does not have an IP address.

## [v1.1.0](https://github.com/ValentinBELYN/icmplib/releases/tag/v1.1.0) - 2020-06-25
- Normalize the names of variables and properties:
  - `ICMPReply` class: the `received_bytes` property is deprecated. Use `bytes_received` instead.
  - `Host` and `Hop` classes: the `transmitted_packets` property is deprecated. Use `packets_sent` instead.
  - `Host` and `Hop` classes: the `received_packets` property is deprecated. Use `packets_received` instead.
- Normalize docstrings.
- Add support for odd size payloads.
- Optimizations.

## [v1.0.4](https://github.com/ValentinBELYN/icmplib/releases/tag/v1.0.4) - 2020-06-14
- Add the `is_closed` property to the `ICMPSocket` class.
- Round round-trip time values by default.
- Fix a bug in the `multiping` function: the `id` parameter was ignored.
- Fix a bug in the `ICMPSocket` class when instantiated without root privileges.
- Add an index for examples.

## [v1.0.3](https://github.com/ValentinBELYN/icmplib/releases/tag/v1.0.3) - 2020-05-09
- Add the ability to customize the payload.
- Improvements of `ping` and `multiping` functions. It is now possible to pass arguments to the `ICMPRequest` object using keywords arguments `**kwargs`.
- Update some docstrings.
- Add new examples.

## [v1.0.2](https://github.com/ValentinBELYN/icmplib/releases/tag/v1.0.2) - 2019-10-20
- Change the license. This project now uses the more permissive license LGPLv3.

## [v1.0.1](https://github.com/ValentinBELYN/icmplib/releases/tag/v1.0.1) - 2019-10-07
- Add some examples.
- Rename `model.py` to `models.py`.
- Update setup keywords.

## [v1.0.0](https://github.com/ValentinBELYN/icmplib/releases/tag/v1.0.0) - 2019-09-29
- :tada: Initial release.
