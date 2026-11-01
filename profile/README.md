# ZeroByte

An open-source, end-to-end encrypted relay for sensitive, private data between
two paired devices. Each update is sealed on the device that sends it. The relay
cannot open it and deletes it once the other device has collected it.

- **No accounts.** Two devices pair once, on the local network.
- **No keys on the relay.** Keys are derived on the devices (HKDF-SHA256) and
  every envelope is sealed with ChaCha20-Poly1305.
- **No request logs.** A mailbox without a write for 30 days erases itself.

| Part | Repository | Licence |
|---|---|---|
| Protocol | [zerobyte-protocol](https://github.com/zerobyte-cloud/zerobyte-protocol): Relay Protocol v1 and test vectors | CC BY 4.0 |
| Relay | [zerobyte-relay](https://github.com/zerobyte-cloud/zerobyte-relay): Node and Cloudflare Workers | AGPL-3.0 |
| SDKs | [Swift](https://github.com/zerobyte-cloud/zerobyte-swift-sdk), [Android](https://github.com/zerobyte-cloud/zerobyte-android-sdk), [JavaScript](https://github.com/zerobyte-cloud/zerobyte-js-sdk), [.NET](https://github.com/zerobyte-cloud/zerobyte-dotnet-sdk) | Apache-2.0 |
| Documentation | [zerobyte-docs](https://github.com/zerobyte-cloud/zerobyte-docs) | CC BY 4.0 |

**Hosted relay.** Run the relay yourself, or use relay.zerobyte.cloud, operated by ZeroByte Cloud
under its [Terms of Service](https://zerobyte.cloud/terms). There, Cloudflare's storage keeps a
30-day history of each mailbox for recovery after a failure; it holds the same sealed envelopes and
nothing more. A relay you run yourself keeps whatever its own storage keeps.

Website: [zerobyte.cloud](https://zerobyte.cloud) ·
Documentation: [docs.zerobyte.cloud](https://docs.zerobyte.cloud) ·
Contact: [hello@zerobyte.cloud](mailto:hello@zerobyte.cloud) ·
Security: [security@zerobyte.cloud](mailto:security@zerobyte.cloud) ·
Abuse: [abuse@zerobyte.cloud](mailto:abuse@zerobyte.cloud) ·
Legal and authorities: [legal@zerobyte.cloud](mailto:legal@zerobyte.cloud)
