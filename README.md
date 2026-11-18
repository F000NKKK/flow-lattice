# Flow Lattice

Rust policy compiler that turns domain, IP, and application rules into platform-neutral network plans for the Lattice networking stack.

## Status

**Bootstrap stage.** This repository currently contains repository workflow,
policies, and packaging scaffolding ported from
[net-lattice](https://github.com/F000NKKK/net-lattice), the first crate in the
Lattice networking ecosystem. The `0.1.0` crate is a placeholder: no policy
compiler or functional public API has landed yet.

The development workspace requires Rust 1.100 or newer.

## The Lattice ecosystem

Net Lattice and DNS Lattice have stable 1.x releases; Tunnel Lattice has
published pre-1.0 releases. Flow Lattice and SDK Lattice remain bootstrap
projects. See each repository for its current release and development status.

| Crate | Purpose |
| --- | --- |
| [net-lattice](https://github.com/F000NKKK/net-lattice) | OS networking inspection and configuration (routes, DNS, interfaces) |
| [tunnel-lattice](https://github.com/F000NKKK/tunnel-lattice) | TUN/TAP tunnel interfaces |
| [dns-lattice](https://github.com/F000NKKK/dns-lattice) | Programmable DNS control plane |
| [flow-lattice](https://github.com/F000NKKK/flow-lattice) | Policy compiler: rules -> platform-neutral network plans |
| [sdk-lattice](https://github.com/F000NKKK/sdk-lattice) | Application-facing SDK composing the crates above |

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Feedback on scope and API direction is
the most valuable contribution at this stage.

## License

Licensed under the [Mozilla Public License 2.0](LICENSE).
