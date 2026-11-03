# click-wheel

Copy MP3 files to an iPod without iTunes.

Status: early development. First target: iPod shuffle 1G and 2G.
Planned v0.1 features: detect device, list tracks, add MP3s, remove tracks.

## Layout

| Path | Role |
|------|------|
| `crates/click-wheel-formats` | Pure codecs. No I/O. |
| `crates/click-wheel-device` | Device file system, model registry, detection. |
| `crates/click-wheel-library` | Service layer. Uses the two crates above. |
| `crates/click-wheel-cli` | Developer tool. |

## Build

```sh
cargo fmt --check
cargo clippy --workspace --all-targets -- -D warnings
cargo test --workspace
```

## License

GPL-3.0-or-later. See `LICENSE` and `NOTICE`.
