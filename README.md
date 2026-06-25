# steam-protobuf

[![node version][node-version]][node-version-href]
[![npm version][npm-version]][npm-version-href]
[![npm downloads][npm-downloads]][npm-downloads-href]

> TypeScript Library for Steam Protobuf Encoding & Decoding

## Installation

```bash
npm install steam-protobuf
```

## Usage

```ts
import { CEconGetTradeOfferAccessTokenRequest } from "steam-protobuf"

// Example payload
const payload = new Uint8Array([0x00])

const decodedPayload = CEconGetTradeOfferAccessTokenRequest
    .decode(payload)

const binaryPayload = CEconGetTradeOfferAccessTokenRequest
    .encode({
        generateNewToken: decodedPayload.generateNewToken
    })
```

## License

[MIT][license-href]

See `LICENSE` for more information.

<!-- Badges -->

[node-version]: https://img.shields.io/badge/Node.js-v24%2B-3366CB?labelColor=171717
[node-version-href]: https://nodejs.org
[npm-version]: https://img.shields.io/npm/v/steam-protobuf?labelColor=171717&color=3366CB
[npm-version-href]: https://npmjs.com/package/steam-protobuf
[npm-downloads]: https://img.shields.io/npm/dm/steam-protobuf?labelColor=171717&color=3366CB
[npm-downloads-href]: https://npmjs.com/package/steam-protobuf
[license-href]: https://github.com/v0eak/steam-protobuf/blob/main/LICENSE