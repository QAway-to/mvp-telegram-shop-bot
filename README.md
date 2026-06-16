# mvp-telegram-shop-bot

> Telegram shop bot UI — product catalog, cart management, and order flow as a Next.js web interface, mirroring the Telegram bot UX.

A Next.js application that replicates the in-chat shopping experience in a browser. Users browse a product catalog, add items to cart, adjust quantities, and place orders. The order flow and bot command structure are designed to map 1-to-1 to a real Telegram Bot API integration.

## Features

- **Product catalog** — grid layout with images, descriptions, and prices
- **Cart** — add, remove, and update quantities with running total
- **Order history** — list of past orders with status and items breakdown
- **Bot UI simulation** — chat-style interaction panels that mirror Telegram UX
- **Responsive design** — Tailwind CSS layout that works on mobile and desktop

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Framework | Next.js 14 (Pages Router) |
| Styling | Tailwind CSS |
| State | React hooks |
| Data | Mock JSON (catalog, orders) |

## Getting Started

```bash
npm install
npm run dev   # http://localhost:3000
```

## Connecting to Telegram

To wire up a real bot, replace the mock data layer with Telegram Bot API calls:

- `POST /bot{token}/sendMessage` for chat responses
- `POST /bot{token}/answerCallbackQuery` for inline button actions
- Webhook endpoint at `/api/telegram` (add to project)

## License

MIT
