# Today I learned

Here’s a list of random things I’ve learned. Take everything with a pinch of salt.

## 2025

### November

- macOS ships with `jq` installed by default – or maybe part of the Command-line Tools for Xcode? Either way, you don’t need to install Homebrew to do things like this:
  ```sh
  curl http://localhost:8000/api/endpoint | jq -r '.message | test("^error"; "i")'
  ```
- It’s [really easy](https://support.apple.com/en-gb/guide/mac-help/mchl91750563/mac) to create a macOS Shortcut to send prompts to the on-device Foundation Model used by Apple Intelligence.
  - You can also set one up to prompt Apple Personal Cloud.
  - I still prefer my [cli tool](https://github.com/liamnewmarch/ai/) though :)
