# Monitor — финансовый дашборд

Сайт с котировками в реальном времени.

**URL:** https://kseniyashev.github.io/monitor/
**Репозиторий:** https://github.com/Kseniyashev/monitor

## Что отслеживает
- USD/RUB — курс доллара к рублю
- BTC/USD — курс биткоина к доллару
- Нефть Brent (BZ=F)
- Золото XAU/USD
- Серебро XAG/USD

По клику на карточку — график за последние 30 дней.
Автообновление каждые 30 секунд.

## API источники
- **USD/RUB live:** open.er-api.com
- **USD/RUB история:** cdn.jsdelivr.net/npm/@fawazahmed0/currency-api
- **BTC:** api.binance.com (через corsproxy.io)
- **Нефть:** Yahoo Finance BZ=F (через corsproxy.io)
- **Золото/Серебро live:** forex-data-feed.swissquote.com (через corsproxy.io)
- **Золото/Серебро история:** Yahoo Finance GC=F / SI=F (через corsproxy.io)

## Как публиковать изменения
Весь сайт — один файл `index.html`. После изменений:
```
git add index.html
git commit -m "описание изменений"
git push
```
GitHub Pages обновится автоматически через ~1 минуту.

## Инструменты
- **gh CLI** установлен через Homebrew (`/usr/local/bin/gh`)
- **GitHub аккаунт:** Kseniyashev
