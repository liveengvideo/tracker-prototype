# Tracker v23.3 — прототип

Единая сборка: 11 групп, 58 экранов.

## Открыть локально

Просто открой `index.html` в браузере (двойным кликом). Никаких зависимостей — это один HTML-файл.

## Опубликовать на GitHub Pages (5 минут)

1. Создай новый репозиторий на GitHub (например, `tracker-prototype`). Можно сделать **публичным** или **приватным** (Pages работает в обоих случаях, но в приватных только на платных тарифах).
2. На своём компьютере открой Terminal и выполни (подставь свой логин):
   ```bash
   cd "/Users/alex29prokhorov/Tracker v23.3/deploy"
   git init
   git add .
   git commit -m "v23.3 prototype"
   git branch -M main
   git remote add origin https://github.com/<твой-логин>/tracker-prototype.git
   git push -u origin main
   ```
3. На GitHub: **Settings → Pages → Build from a branch → main → / (root) → Save**.
4. Через 1–2 минуты по адресу `https://<твой-логин>.github.io/tracker-prototype/` будет открываться прототип.

## Поделиться без техдеталей

Добавь к ссылке `?public=1`, чтобы спрятать meta-блоки (статус, спека, audit-notes):

```
https://<твой-логин>.github.io/tracker-prototype/?public=1
```

Получатель может включить техдетали обратно чекбоксом в шапке.

## Альтернативы (если без GitHub Pages)

- **Netlify Drop**: https://app.netlify.com/drop — перетащи папку `deploy/`, получи URL.
- **Vercel**: https://vercel.com/new — drag & drop.
- **Cloudflare Pages**: https://pages.cloudflare.com — связать с git-репозиторием.

## Обновление после правок

Если опубликовал через GitHub Pages — после правок в `index.html`:
```bash
git add index.html
git commit -m "update"
git push
```
GitHub Pages обновится за 1–2 минуты.

## Прямые ссылки на экраны

URL-формат якорей (через `#`, а не `?`):
- `…/#screen-04` — конкретный экран (S1 главный)
- `…/#group-2` — группа (Дневник)
- `…/#toc` — оглавление
- `…/#top` — самый верх

Можно совмещать с режимом без техдеталей: `…/?public=1#screen-04`.

