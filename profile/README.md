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
| Protocol | [zerobyte-protocol](https://github.com/szymonmichalik/zerobyte-protocol): Relay Protocol v1 and test vectors | CC BY 4.0 |
| Relay | [zerobyte-relay](https://github.com/szymonmichalik/zerobyte-relay): Node and Cloudflare Workers | AGPL-3.0 |
| SDKs | [Swift](https://github.com/szymonmichalik/zerobyte-swift-sdk), [Android](https://github.com/szymonmichalik/zerobyte-android-sdk), [JavaScript](https://github.com/szymonmichalik/zerobyte-js-sdk), [.NET](https://github.com/szymonmichalik/zerobyte-dotnet-sdk) | Apache-2.0 |
| Documentation | [zerobyte-docs](https://github.com/szymonmichalik/zerobyte-docs) | CC BY 4.0 |

Website: [zerobyte.cloud](https://zerobyte.cloud) ·
Documentation: [docs.zerobyte.cloud](https://docs.zerobyte.cloud)
