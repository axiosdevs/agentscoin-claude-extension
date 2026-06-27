# AgentsCoin — Claude Desktop Extension 🪙

**Give Claude its own crypto wallet.** One-click [Claude Desktop](https://claude.ai/download) extension for **[AgentsCoin](https://agents-coin.com)** — a live EVM chain built for AI agents. From the chat, Claude can create a wallet, get AGENT from the faucet, check balance, send, and **create + trade tokens**.

## Install (one click)
1. Download **[agentscoin.mcpb](https://github.com/axiosdevs/agentscoin-claude-extension/releases/latest/download/agentscoin.mcpb)** (or the file in this repo).
2. Claude Desktop → **Settings → Extensions** → drag in `agentscoin.mcpb` (or *Install from file*).
3. Enable it. Done — **8 tools**.

> `.mcpb` is Claude Desktop's extension format — open it **inside** Claude Desktop, not by double-clicking.

**No-install alternative (remote, no warnings):** Settings → **Connectors → Add custom connector** → `https://agents-coin.com/mcp`

## How to use (just chat with Claude)
**First run**
- *"Show AgentsCoin network info"* — confirms it works.
- *"Create an AgentsCoin wallet"* — returns an address + private key (save it!).
- *"Get AGENT from the faucet to 0x…"* — funds the wallet **instantly, in the chat** (no browser). Needed for gas.
- *"Check the balance of 0x…"*

**Create & trade a token** (a pump.fun for agents)
- *"Create a token DogeAI (DOGE) on AgentsCoin using key 0x…"* → token address + explorer link.
- *"Add liquidity: 1000 DOGE + 5 AGENT, key 0x…"*
- *"Buy token 0x… for 5 AGENT, key 0x…"* · *"Sell 100 of token 0x…"*

**Send** — *"Send 1 AGENT to 0x… from key 0x…"*

## The 8 tools
`network_info` · `create_wallet` · `mine` (faucet, in-chat) · `balance` · `send` · `create_coin` · `add_liquidity` · `swap`

## Notes
- **Gas first:** fund a fresh wallet via *mine* (faucet) before send / create / swap.
- **Keys:** `create_wallet` returns the private key in plain text — keep it out of shared chats for any wallet you actually fund.
- Network: **AgentsCoin** · chainId **24368** · explorer https://explorer.agents-coin.com · DEX https://dex.agents-coin.com

## Links
- 🌐 Site: https://agents-coin.com
- 🧩 MCP source + other clients (npx, pip, AgentKit, n8n, ElizaOS): https://github.com/axiosdevs/agentscoin-mcp

MIT.

## Privacy Policy

Full policy: https://agents-coin.com/privacy.html — The extension collects **no** personal data; wallet keys are generated and stored **only locally** (`~/.agentscoin/wallets.json`) and never sent to us. It talks only to the public AgentsCoin RPC / faucet / explorer to perform actions you initiate. Contact: asodevx@gmail.com
