# Today I learned

Here’s a list of random things I’ve learned. Take everything with a pinch of salt.

## 2026

### January

- Wikipedia have a meta guide on how to detect the [signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing).
- You can use [What’s up Docker](https://getwud.github.io/wud/) to get notifications when new images are available.
  - Previously I used Watchtower to keep containers up to update, but this allows me to check the changelogs first.
- [Helix](https://github.com/helix-editor/helix/) has support for code generation via [LSP-AI](https://github.com/SilasMarvin/lsp-ai).
  - For context; Helix doesn’t have plugins, instead you configure language servers to analyze, lint and format your code.

## 2025

### December

- Linus Torvalds builds [guitar pedals](https://github.com/torvalds/GuitarPedal) for fun, despite not playing guitar.
  > Also, because I don't typically listen to the end result, but look at it with a signal generator and an oscilloscope, I've grown to detest power supply noise.

### November

- Node.js has support for SQLite right out of the box:
  ```js
  import { DatabaseSync } from 'node:sqlite'

  const db = new DatabaseSync(':memory:')
  db.exec('CREATE TABLE users (id INT, name TEXT)')
  ```

- macOS ships with `jq` installed by default – or maybe part of the Command-line Tools for Xcode? Either way, you don’t need to install Homebrew to do things like this:
  ```sh
  curl http://localhost:8000/api/endpoint | jq -r '.message | test("^error"; "i")'
  ```

- You can [use Apple Shortcuts to chat](https://support.apple.com/en-gb/guide/mac-help/mchl91750563/mac) with the LLMs which power Apple Intelligence.
  - Prompts are handled locally by the on-device Foundation Model.
  - For more complex prompts you can also chat with Apple Personal Cloud.
  - I still prefer my [cli tool](https://github.com/liamnewmarch/ai/) though :)
