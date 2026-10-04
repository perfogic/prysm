### Fixed

- Read the `tcp6`, `quic6` and `udp6` ENR entries when building a peer's IPv6 addresses, so peers that advertise only `tcp6` are dialed and dual-stack peers are dialed on their IPv6 port.
