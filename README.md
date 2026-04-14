# @discordjs/opus

> Native bindings to libopus v1.5

This fork targets macOS only and builds from source during installation with `node-gyp`.

## Usage

```js
import { OpusEncoder } from '@discordjs/opus';

// Create the encoder.
// Specify 48kHz sampling rate and 2 channel size.
const encoder = new OpusEncoder(48_000, 2);

// Encode and decode.
const encoded = encoder.encode(buffer);
const decoded = encoder.decode(encoded);
```

## Platform support

⚠ Node.js 24.x on macOS is required.

- macOS x64
- macOS arm64
