# BlackLabr

Одностраничный сайт продуктовой студии — делаем собственные мобильные приложения.
Просто и со вкусом.

## Стек
- HTML + [Tailwind CSS](https://tailwindcss.com/) (через CDN — сборка не нужна)

## Структура
- `index.html` — главная: логотип, слоган, список приложений, блок компании
- `policies/privacy.html` — политика компании BlackLabr Limited (сайт)
- `policies/fishing-app-privacy.html` — политика продукта Fishing App
- `favicon.ico`, `assets/` — иконки и логотип
- `CNAME` — кастомный домен (blacklabr.com)

## Запуск локально
Откройте `index.html` в браузере. Или поднимите статический сервер:

```bash
python3 -m http.server 8000
```

Затем откройте http://localhost:8000

## Деплой
Репозиторий называется `blacklabr.github.io`, поэтому GitHub Pages автоматически
публикует `index.html` из ветки `main` на https://blacklabr.github.io после `git push`.

## Что менять
- Приложения — блоки в секции «Our apps» в `index.html` (название, описание, ссылки Website / iOS / Android / Privacy)
- Контакты — `info@blacklabr.com` и `support@blacklabr.com` (заглушки, замените на реальные)
- Дата в privacy policy — строка «Effective date»
- Цвет бренда — `colors.brand` в конфиге Tailwind в `<head>` (сейчас `#27C1FE`)
