# Atomic Gitmoji

A Codex plugin that organizes mixed changes into small, focused Git commits with Unicode Gitmoji messages.

## Install in Codex

Add this GitHub repository as a marketplace.

```sh
codex plugin marketplace add igorcamilo/atomic-gitmoji --ref main
```

In the ChatGPT desktop app, open Plugins, select the **Atomic Gitmoji** marketplace, and install **Atomic Gitmoji**. Start a new Codex session to use it. A private repository requires working Git credentials.

## Refresh from Git

Codex can refresh a Git-backed marketplace automatically. To request a refresh explicitly after a push, run:

```sh
codex plugin marketplace upgrade atomic-gitmoji
```

See [OpenAI's plugin packaging guide](https://developers.openai.com/plugins/build/plugins) for marketplace setup.
