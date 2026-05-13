# CORE PANIC

Готовый минимальный Phaser 3 проект для Яндекс Игр.

## Запуск локально
Открой папку через локальный сервер:

```bash
python -m http.server 8080
```

Потом открой `http://localhost:8080`.

Локально `/sdk.js` не загрузится, это нормально: игра включит fallback и будет работать без Яндекс SDK.

## Загрузка на Яндекс Игры
Загружай архив с `index.html`, `src/` и `lib/` в корне архива.

## Что уже встроено
- Phaser 3 локально в `lib/phaser.min.js`
- Yandex SDK через `/sdk.js`
- `YaGames.init()`
- `ysdk.features.GameplayAPI.start/stop`
- fullscreen-реклама после смерти
- rewarded-реклама за стартовый буст/продолжение
- сохранение рекорда через `player.setData`, fallback в `localStorage`
- отправка рекорда в лидерборд `core_panic_score`
- полностью кодовый визуал, без PNG и внешних ассетов
- управление ПК и мобилка

## В консоли Яндекс Игр
Создай leaderboard с техническим именем:

`core_panic_score`

Тип сортировки: чем больше, тем лучше.
