

# Liteanime API

[![Лицензия](https://img.shields.io/badge/Лицензия-MIT-green.svg)](LICENSE)

**Liteanime API** — это открытый репозиторий, предоставляющий структурированные данные об аниме. Наша цель — предложить лёгкий и доступный набор данных для разработчиков, энтузиастов и любителей аниме.

Данные доступны в двух популярных форматах: **CSV** и **JSON**. Вы можете использовать их непосредственно из этого репозитория или с сервера API (если он доступен).

## 📦 Форматы данных

*   **CSV** — `anime_data.csv` (удобен для электронных таблиц и анализа данных)
*   **JSON** — `anime_data.json` (идеален для веб-приложений, скриптов и API)

## 🚀 Как использовать данные

### Способ 1. Прямая загрузка из репозитория GitHub
Скачайте файлы вручную по ссылкам:
*   [anime_data.csv](https://github.com/liteanimeru/api-liteanime/blob/main/anime_data.csv)
*   [anime_data.json](https://github.com/liteanimeru/api-liteanime/blob/main/anime_data.json)

### Способ 2. Получение через `raw.githubusercontent.com`
Используйте прямые ссылки на последнюю версию файлов в своём коде:
```
https://raw.githubusercontent.com/liteanimeru/api-liteanime/main/anime_data.json
https://raw.githubusercontent.com/liteanimeru/api-liteanime/main/anime_data.csv
```

**Пример на JavaScript:**
```javascript
fetch('https://raw.githubusercontent.com/liteanimeru/api-liteanime/main/anime_data.json')
  .then(response => response.json())
  .then(data => console.log(data));
```

### Способ 3. Клонирование репозитория
Получите полную историю изменений и все файлы:
```bash
git clone https://github.com/liteanimeru/api-liteanime.git
```

### Способ 4. Использование сервера `api.liteanime.ru`

*   CSV: [`http://api.liteanime.ru/anime_data.csv`](http://api.liteanime.ru/anime_data.csv)
*   JSON: [`http://api.liteanime.ru/anime_data.json`](http://api.liteanime.ru/anime_data.json)

Пример запроса:
```javascript
fetch('http://api.liteanime.ru/anime_data.json')
  .then(response => response.json())
  .then(data => console.log(data));
```

## 📊 Структура данных

Файлы содержат массив объектов, каждый из которых описывает одно аниме. Ниже приведены типичные поля, которые присутствуют в данных (точный набор можно узнать, скачав файлы):

| Поле | Описание | Пример |
| :--- | :--- | :--- |
| `anime_id` | Уникальный идентификатор | `12345` |
| `title` | Основное название | «Shingeki no Kyojin» |
| `title_english` | Английское название | «Attack on Titan» |
| `title_japanese` | Японское название | «進撃の巨人» |
| `synopsis` | Краткое описание сюжета | текст |
| `genre` | Список жанров | «Action, Drama, Fantasy» |
| `episodes` | Количество серий | `25` |
| `status` | Статус трансляции | «Finished Airing» |
| `aired_from` | Дата начала показа | `2013-04-07` |
| `aired_to` | Дата окончания показа | `2013-09-29` |
| `rating` | Средняя оценка | `8.5` |
| `image_url` | Ссылка на постер | `https://...` |
| `studios` | Студия / студии | «Wit Studio» |

> **Примечание:** Это лишь пример возможной структуры. Актуальную схему всегда можно посмотреть непосредственно в файлах `anime_data.csv` или `anime_data.json`.

## 💡 Возможные применения

*   Создание собственной базы данных аниме или приложения-каталога.
*   Тренировка навыков анализа данных (Python, R, Excel).
*   Наполнение тестового окружения для веб-проектов.
*   Генерация статического сайта с информацией об аниме.

## 🤝 Как помочь проекту

Мы приветствуем вклад сообщества! Если вы хотите улучшить данные:

1. **Сделайте форк** (fork) репозитория.
2. Внесите изменения в файлы (например, исправьте опечатки, обновите информацию).
3. Отправьте **пул-реквест** (pull request) с понятным описанием ваших правок.

Пожалуйста, старайтесь, чтобы ваши дополнения были точными и соответствовали текущей структуре данных.

## 📜 Лицензия

Проект распространяется под лицензией **MIT**. Вы можете свободно использовать данные в своих проектах, в том числе коммерческих. Подробности — в файле [LICENSE](LICENSE).


---

Если у вас есть вопросы или предложения, создавайте **Issue** в этом репозитории. Приятного использования!
