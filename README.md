# garage-ai-bot

Telegram-бот + Mini App: фотографируешь машину — ИИ определяет
марку/модель/год и считает оценку уникальности (0-100) по
фиксированному алгоритму, карточка машины сохраняется в твой
личный "гараж".

Пет-проект для себя и друзей, некоммерческий.

## Структура проекта

- [`docs/plan.md`](./docs/plan.md) — план разработки: идея, стек, этапы
- [`docs/uniqueness-algorithm.md`](./docs/uniqueness-algorithm.md) — алгоритм оценки уникальности машины
- `backend/` — бот (Python + python-telegram-bot) + API + интеграция с vision-моделью + БД
- `miniapp/` — Telegram Mini App (фронтенд "гаража")

## Стек

- **Бот/бэкенд:** Python + [python-telegram-bot](https://github.com/python-telegram-bot/python-telegram-bot) (async)
- **Mini App:** JS/TS (Node/React), UI в стиле Liquid Glass
- **БД:** PostgreSQL (SQLite на старте)
- **AI (vision):** GigaChat + Google Gemini как бэкап

Подробности — в [`docs/plan.md`](./docs/plan.md).
