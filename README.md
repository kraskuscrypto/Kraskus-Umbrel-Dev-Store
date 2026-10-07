# Kraskus Crypto (Dev) — Umbrel App Store

**Testing channel.** Umbrel-native store with Kraskus apps from the 5tratumOS Dev store
[`Kraskus-Crypto-Dev-Store`](https://github.com/kraskuscrypto/Kraskus-Crypto-Dev-Store).
Customers should use [`Kraskus-Umbrel-Store`](https://github.com/kraskuscrypto/Kraskus-Umbrel-Store).

**Add only one Kraskus store, this one or the production store, never both.** Both use the
store id `kraskus`, because Umbrel requires app IDs to start with the store id. They share app
IDs, and Umbrel installs a shared app from whichever store was added first, so with both added
you can silently get the other channel's version.

The app folders are generated. Do not edit them here; the generator, validator and Umbrel copy
overrides live in `Kraskus-Umbrel-Store/tools/umbrel-store-gen/`. `generated-from.json` records the source commit.

**Common Foundry GPU Miner** requests GPU access through Umbrel's `permissions: [GPU]`.
It installs on any host; mining needs an NVIDIA GPU with the driver loaded.
