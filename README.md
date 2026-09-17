# Russian Language Pack for Publii / Русская локализация для Publii

Русский языковой пакет для [Publii](https://getpublii.com) — десктопной CMS для создания статических сайтов.

Russian UI translation for [Publii](https://getpublii.com), a desktop CMS for building static websites.

---

## Details / Характеристики

| Параметр | Значение |
|---|---|
| **Name** | Русская - локализация (`ru-ru`) |
| **Version** | 1.8.1 |
| **Publii Support** | 0.47.0+ |
| **WYSIWYG Translation** | ✅ Yes (`wysiwyg.json` included) |
| **Contents** | `config.json`, `translations.json`, `wysiwyg.json`, `thumbnail.svg` |

> Файл `ru-ru.zip` — это готовый к установке пакет интерфейса Publii. Распаковывать его вручную не нужно.

## Installation / Установка

Официальная инструкция Publii: [Changing Publii's Language](https://getpublii.com/docs/changing-publiis-language.html). Перевод интерфейса и перевод темы сайта — это разные вещи (этот репозиторий — про интерфейс программы).

### Порядок установки (через интерфейс Publii — рекомендуется)

1. Скачайте файл **`ru-ru.zip`** со страницы [Releases](../../releases) этого репозитория (раздел Assets). Не распаковывайте архив.
2. Откройте приложение **Publii**.
3. Нажмите на кнопку **меню (⋮ / три точки)** в правом верхнем углу.
4. Выберите пункт **Languages / Языки**.
5. Нажмите кнопку **Install Language** вверху экрана — откроется проводник.
6. Найдите скачанный файл `ru-ru.zip` и выберите его (двойной клик).
7. Язык появится в списке на экране Languages — **кликните по «Русский»**, чтобы сделать его активным.
8. Перезапустите Publii, если интерфейс переключился не полностью.

Готово — интерфейс Publii будет на русском языке.

### Видео/скриншоты-подсказки

- `⋮ → Languages → Install Language → выбрать ru-ru.zip → кликнуть по языку`

### Ручная установка (если кнопка Install Language не срабатывает)

Если при установке возникает ошибка (например, известная `EEXIST ... __TEMP__`, см. [GetPublii/Publii#1105](https://github.com/GetPublii/Publii/issues/1105)):

1. Закройте Publii.
2. Найдите папку языков Publii:
   - Windows: `Документы\Publii\languages\`
   - macOS: `~/Documents/Publii/languages/`
   - Linux: `~/Documents/Publii/languages/`
3. Распакуйте `ru-ru.zip` так, чтобы получилась папка `.../languages/ru-ru/` с файлами `config.json`, `translations.json`, `wysiwyg.json`.
4. Запустите Publii → `⋮ → Languages` → выберите Русский.

### Важно: язык интерфейса ≠ язык сайта

- Этот пакет переводит **только интерфейс программы Publii** (меню, настройки, редактор).
- Язык самого создаваемого сайта (HTML `lang`, даты, тексты темы) настраивается отдельно: **Site Settings → Language** + файлы перевода темы (`theme.lang.json`). См. [How to translate your Publii theme](https://getpublii.com/docs/translate-publii-theme-to-another-language.html).

## Repository structure / Структура репозитория

```text
.
├── ru-ru.zip       # готовый языковой пакет для установки через Publii
├── README.md
├── LICENSE         # MIT
└── .gitignore
```

Исходники пакета (внутри zip): `ru-ru/config.json`, `ru-ru/translations.json`, `ru-ru/wysiwyg.json`, `ru-ru/thumbnail.svg`.

## Compatibility / Совместимость

- Проверено с `publiiSupport: 0.47.0`, версия пакета `1.8.1`.
- Для новых версий Publii (0.47.x / 0.48+) пакет обычно продолжает работать; недостающие строки Publii покажет на английском. Актуальность можно проверить инструментом [Language File Checker](https://getpublii.github.io/language-file-checker/).

## Contributing / Как помочь

Нашли опечатку или непереведённую строку?

1. Сравните `translations.json` с базовым английским через [Language File Checker](https://getpublii.github.io/language-file-checker/).
2. Откройте Issue или Pull Request с исправлением.
3. Пересоберите `ru-ru.zip` (корень архива → папка `ru-ru/` с 4 файлами) и приложите к PR/Release.

Апстрим всех локализаций: [GetPublii/Publii-ui-locales](https://github.com/GetPublii/Publii-ui-locales).

## License / Лицензия

[MIT](LICENSE). См. файл `LICENSE`.

## Links / Ссылки

- Publii: <https://getpublii.com>
- Документация по смене языка: <https://getpublii.com/docs/changing-publiis-language.html>
- Все официальные локализации: <https://github.com/GetPublii/Publii-ui-locales>
