# Construct Event Mini App (MVP)

## Що зроблено

- `/construct_event` у ЛС тепер показує кнопку `🧩 Відкрити Mini App` (якщо задано URL).
- Mini App надсилає дані в бот через `Telegram.WebApp.sendData(...)`.
- Бот приймає `web_app_data` і зберігає базові налаштування:
  - `buffs_enabled`
  - `unique_buffs_only`
  - `registration_time`

## Налаштування

Потрібно задати один з env:

- `CONSTRUCT_EVENT_WEBAPP_URL=https://your-domain/construct-event`
- або `WEBAPP_BASE_URL=https://your-domain` (бот сам додасть `/construct-event`)

Важливо: URL має бути `https`.

## Розміщення front-end

Файл:

- `miniapp/construct-event/index.html`

Його треба віддати як статичний файл за шляхом `/construct-event`.

