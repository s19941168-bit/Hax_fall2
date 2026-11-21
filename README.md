# Hex Fall 3D — мобильная сборка

## Как получить APK
1. Создай на GitHub новый репозиторий.
2. Загрузи в него ВСЁ содержимое этой папки (включая скрытую папку `.github`).
3. Открой вкладку **Actions** → **Build Android APK** → **Run workflow** (или просто сделай push).
4. Через 5–10 минут открой завершённый запуск → внизу **Artifacts** → скачай `HexFall-apk`.
5. Распакуй архив, перекинь `app-debug.apk` на телефон и установи (разреши установку из неизвестных источников).

## Обновить игру
Замени файл `www/index.html` и сделай commit — APK соберётся заново.

## Структура
- `www/index.html` — сама игра
- `assets/` — иконка игры (icon-only, icon-foreground, icon-background)
- `capacitor.config.json`, `package.json` — настройки приложения
- `.github/workflows/build-apk.yml` — автосборка APK
