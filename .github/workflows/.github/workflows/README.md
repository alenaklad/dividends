# Дивиденды РФ — GitHub Pages сайт

- Скрейп данных с dohod.ru по расписанию (каждый час).
- Фронтенд Vite + React: таблица, экспорт CSV/Excel, графики, переключатель темы.
- Публикация в GitHub Pages (Actions).

## Быстрый старт
1. Создай репозиторий **dividends** и включи Settings → Pages → Build and deployment → Source: **GitHub Actions**.
2. Скопируй файлы из этого проекта в корень репозитория.
3. Коммит в ветку `main` — сайт соберётся и опубликуется на GitHub Pages.
4. Workflow **Scrape & Deploy (hourly)** будет обновлять `data/dividends.json` и деплоить.

## Локально
```bash
# скрейп
cd scripts && pnpm install && cd ..
node scripts/scrape.mjs

# фронтенд
cd frontend && pnpm install && pnpm dev
