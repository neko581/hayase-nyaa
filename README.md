# Hayase Nyaa Extension

A fast and reliable **Nyaa.si** search extension for **Hayase** (formerly Miru).

## Features

- Direct search on nyaa.si using its official RSS endpoint
- Intelligent release type detection:
  - `best` — Trusted uploaders & high-quality encodes (1080p, 2160p, BluRay, HEVC, etc.)
  - `batch` — Complete seasons and batch releases
  - `alt` — Everything else
- Returns full torrent info: magnet link, hash, seeders, size (in bytes), date, etc.
- Zero external dependencies — pure JavaScript
- Full TypeScript IntelliSense support via JSDoc

## Installation

1. Open **Hayase** → **Settings** → **Extensions** → **Repositories**
2. Add the repository:
   ```
   https://raw.githubusercontent.com/neko581/hayase-nyaa/main/index.json
   ```
3. Press Import Extensions

## Usage

The extension exposes a `Nyaa` class with the following methods:

- `single({ titles, episode })`
- `batch(...)` / `movie(...)` — Aliases for `single`

It automatically returns results compatible with Hayase's `TorrentResult` interface.

## Credits

Built for the Hayase community.

Feel free to open issues or contribute improvements!

## License

Licensed under the [WTFPL](http://www.wtfpl.net/) — Do What The Fuck You Want To Public License.