# 4x4 Sudoku

A simple, mobile-friendly 4x4 Sudoku game built with Vue.js 3.

🎮 **Play now:** [sudoku4.yeepily.com](https://sudoku4.yeepily.com)

## Features

- 🧩 Random 4x4 Sudoku puzzle generation with unique solutions
- ✅ Real-time input validation
- ⏱️ Timer with best time tracking (persisted in localStorage)
- ↩️ Undo functionality
- 🎨 Optional color hints for visual feedback
- 🌍 Multi-language support:
  - English
  - 中文 (Chinese Traditional)
  - 简体中文 (Chinese Simplified)
  - 日本語 (Japanese)
  - Español (Spanish)
- 📱 Mobile-friendly responsive design
- ⚙️ Settings modal with hamburger menu

## Project Structure

```
sudoku4/
├── public/
│   └── index.html    # Single-file Vue.js application
├── worker.js         # Cloudflare Worker entry point
├── wrangler.toml     # Cloudflare Workers configuration
└── README.md
```

## Local Development

Simply open `public/index.html` in your browser to start playing locally. No build step required!

## Deployment

This project is configured for deployment on [Cloudflare Workers](https://workers.cloudflare.com/) with static assets.

### Prerequisites

- [Node.js](https://nodejs.org/)
- [Wrangler CLI](https://developers.cloudflare.com/workers/wrangler/install-and-update/)

### Deploy

```bash
# Install Wrangler if you haven't already
npm install -g wrangler

# Login to Cloudflare
wrangler login

# Deploy to Cloudflare Workers
wrangler deploy
```

The app will be deployed to your configured custom domain or the default `*.workers.dev` subdomain.

## How to Play

1. Fill in the empty cells with numbers 1-4
2. Each row must contain the numbers 1-4 without repetition
3. Each column must contain the numbers 1-4 without repetition
4. Each 2x2 box must contain the numbers 1-4 without repetition
5. Try to complete the puzzle as fast as you can!

## License

MIT