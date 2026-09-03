# Лендинг книги

Статичний односторінковий сайт для GitHub Pages. Він не потребує збірки, пакетного менеджера або серверної частини.

## Перед публікацією

У `index.html` замініть чотири входження `REPLACE_WITH_SITE_URL` на повну адресу сайту без завершального `/`.

PDF уже підключений локально як `assets/whose-productivity-ivan-bondar-ua.pdf`.

Наприклад:

- сайт: `https://username.github.io/book-name`;
- PDF: `https://username.github.io/book-name/assets/whose-productivity-ivan-bondar-ua.pdf`.

Щоб оновити книгу без зміни посилання на сайті, замініть PDF новою версією з тією самою назвою файлу.

## Публікація в окремому репозиторії

1. Скопіюйте весь вміст папки `website/` у корінь нового публічного репозиторію.
2. Замініть два placeholder-значення, описані вище.
3. У налаштуваннях репозиторію відкрийте **Settings → Pages**.
4. У **Build and deployment** виберіть **Deploy from a branch**.
5. Виберіть гілку `main` і папку `/ (root)`.
6. Після появи URL перевірте завантаження PDF і прев'ю посилання.

## Локальний перегляд

Відкрийте `index.html` напряму або запустіть у цій папці простий статичний сервер:

```sh
python3 -m http.server 4173
```

## Файли

- `index.html` — зміст і metadata;
- `styles.css` — адаптивний дизайн;
- `assets/og-book.png` — прев'ю для LinkedIn і Telegram;
- `assets/favicon.svg` — іконка вкладки.
