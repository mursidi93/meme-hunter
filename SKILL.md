---
name: Meme Hunter Pro
description: AI trading skill powered by onchainOS for discovering meme opportunities
version: 1.0
author: Mukidi Labs
tools:
  - onchainOS

trigger_keywords:
  - trending meme
  - smart money buy
  - low cap meme
  - meme under 10M
  - hot Solana meme

output_format:
  - Token
  - Chain
  - Market Cap
  - Volume
  - Holders
  - Risk
  - Reason
  - Suggested Action
---

# Meme Hunter Pro

Purpose:
Find meme opportunities using onchainOS as primary data source.

## Error Handling

If onchainOS data is unavailable:

1. Notify user that primary source is unavailable
2. Retry scan once
3. Return partial findings if available
4. Avoid generating unsupported trading claims

Fallback:

"No matching opportunities found under current filters. Try increasing market cap range or reducing constraints."
