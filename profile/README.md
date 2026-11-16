<p align="center">
  <img src="https://avatars.githubusercontent.com/u/241353095?v=4" alt="ZcashMe" width="120" />
</p>

## Welcome to ZcashMe

ZcashMe runs the Zcash Name Service, a way to pay someone on Zcash by name instead of by a long shielded address.

Our goal is to make private money as easy to send as a message, without asking anyone to trust us with their names or their payments.

## ZcashNames

[ZcashNames](https://zcashnames.com) lets anyone register a short name, like `alice`, that points at a shielded Zcash address. It went live on mainnet on October 15, 2026.

ZcashNames is built from three parts:

1. Names are recorded on Zcash itself, as Name Notes in the Ironwood shielded pool, and each note commits to its name, its address and the note it replaced.
2. The mint that writes those notes runs inside a trusted execution environment, next to a Zebra full node, and its seed is sealed to that environment.
3. The registry's viewing key is public, so anyone can run a resolver and check every name for themselves.

- [Whitepaper](https://zcashme.github.io/zns-whitepaper/): A Deterministic, Attested Name Registry on Zcash
- [zns-mint](https://github.com/zcashme/zns-mint): The mint
- [zns-resolver](https://github.com/zcashme/zns-resolver): The resolver, with SDKs for TypeScript, Dart and Rust
- [zns-verify](https://github.com/zcashme/zns-verify): The verification kernel for Name Note commitments
- [zns-zcash_primitives](https://github.com/zcashme/zns-zcash_primitives) and [orchard](https://github.com/zcashme/orchard): Name Note support in the Zcash transaction builder
- [zns-deployment](https://github.com/zcashme/zns-deployment): The reproducible image the mint runs in
