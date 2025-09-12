# Zhigalov Landing

Готовый статический лэндинг для GitHub Pages.

## Файлы
- `index.html` — разметка
- `styles.css` — стили
- `portrait.png` — фото
- `Zhigalov_Publications.pdf` — публикации (кликабельная ссылка в блоке «Наукометрия»)
- `robots.txt` — запрет индексации (noindex, nofollow)
- `.nojekyll` — отключение Jekyll на GitHub Pages

## Публикация на GitHub Pages (быстрый путь)
1. Создайте новый репозиторий на GitHub, например `landing`.
2. Загрузите сюда все файлы из этой папки (через Upload files).
3. Откройте Settings → Pages → **Build and deployment**:
   - Source: `Deploy from a branch`
   - Branch: `main` / `/ (root)` → Save
4. Через 1–2 минуты появится ссылка вида: `https://<ваш-логин>.github.io/landing/`

### Вариант с git
```bash
git init
git add .
git commit -m "Initial landing"
git branch -M main
git remote add origin https://github.com/<ваш-логин>/landing.git
git push -u origin main
```
Затем включите Pages, как указано выше.

## Noindex
`<meta name="robots" content="noindex, nofollow">` уже добавлен в `<head>`, а в корне есть `robots.txt` с `Disallow: /`.
