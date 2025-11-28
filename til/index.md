# Today I learned

Here’s a list of random things I’ve learned. Take everything with a pinch of salt.

## 2025

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

- It’s [really easy](https://support.apple.com/en-gb/guide/mac-help/mchl91750563/mac) to use macOS Shortcuts to chat with Apple Intelligence.
  - Prompts are handled locally by the on-device Foundation Model.
  - For more complex prompts you can also chat with Apple Personal Cloud.
  - I still prefer my [cli tool](https://github.com/liamnewmarch/ai/) though :)
