# tectec for Claude Code

Connects Claude Code to your [tectec](https://tectec.app) account: find recipes in your library, import them from links, photos or pasted text, edit recipes and books, plan menus and combine them into a grocery list.

## Install

```sh
claude plugin install tectec --marketplace guillaq/tectec
```

Or from inside Claude Code:

```
/plugin marketplace add guillaq/tectec
/plugin install tectec@tectec
```

Then run `/mcp`, pick **tectec** and authenticate. Your browser opens tectec, where you sign in, check what Claude Code is asking for and choose **connect**. No API key is needed.

## Without the plugin

tectec is a remote MCP server at `https://tectec.app/api/mcp`, so any assistant that supports remote MCP servers with sign-in can use it:

```sh
claude mcp add --transport http tectec https://tectec.app/api/mcp
```

Setup for Codex, Claude, ChatGPT and others is in the [tectec docs](https://tectec.app/docs#connecting-an-ai-assistant).

## Privacy

The plugin holds no credentials. Sign-in happens on tectec.app, the assistant only gets what you approve on the consent page, and you can disconnect it at any time in [settings](https://tectec.app/settings) under **connected apps**.
