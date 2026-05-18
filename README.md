# Архивирование в Linux

Статический сайт на [GitHub Pages](https://pages.github.com/) (Jekyll + тема Cayman).

## Публикация

1. Создайте репозиторий на GitHub и отправьте туда этот проект.
   - Чтобы сайт открывался как **`https://ВАШ_ЛОГИН.github.io/`** (без пути `/репо/`), репозиторий **обязан** называться ровно **`ВАШ_ЛОГИН.github.io`** (например, `zenc0dr.github.io`). Если репозиторий называется иначе (например, `c0dr`), сайт будет по адресу **`https://ВАШ_ЛОГИН.github.io/c0dr/`**, а корень `github.io` даст **404**.
2. В репозитории: **Settings → Pages → Build and deployment → Source**: ветка `main` (или `master`), папка **`/` (root)**.
3. Если адрес сайта будет **`https://ВАШ_ЛОГИН.github.io/ИМЯ-РЕПО/`** (обычный проектный Pages), откройте **`_config.yml`** и задайте:
   - `baseurl: "/ИМЯ-РЕПО"` — ровно как репозиторий называется, со слэшем в начале;
   - при желании `url: "https://ВАШ_ЛОГИН.github.io"`.
4. Если репозиторий называется **`ВАШ_ЛОГИН.github.io`**, сайт откроется в корне домена — оставьте `baseurl: ""` и при необходимости укажите `url`.

После первого деплоя подождите минуту-две и откройте URL из вкладки Pages.

## Локальная проверка (по желанию)

Нужны Ruby и Jekyll; см. [документацию GitHub](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll).
