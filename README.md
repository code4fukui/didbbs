# didbbs

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A bulletin board system (BBS) that uses Decentralized Identifiers (DIDs) for authentication.

## Demo
- [DID BBS](https://didbbs.code4fukui.org)

## Features
- Post messages anonymously using a DID and digital signature
- View a list of all messages posted

## Requirements
- Deno runtime environment

## Usage
1. Clone the repository
2. Run the server using Deno: `deno run --allow-net --allow-read --allow-write didbbs.js`
3. Open the web application in a browser at `http://localhost:8001`

## Data / API
- The BBS data is stored in a JSON file named `bbs.json`
- The server provides two API endpoints:
  - `/api/list`: Returns the list of all BBS messages
  - `/api/add`: Adds a new message to the BBS, requires a valid DID and digital signature

## License
MIT License — see [LICENSE](LICENSE).