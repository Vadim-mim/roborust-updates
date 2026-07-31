# Новости RoboRust

## Первая настройка

1. Открой репозиторий `Vadim-mim/roborust-updates`.
2. Загрузи папку `news` из этого архива целиком в корень репозитория.
3. Убедись, что адрес существует:
   `https://raw.githubusercontent.com/Vadim-mim/roborust-updates/main/news/news.json`
4. Запусти лаунчер и нажми `Новости` → `Обновить новости`.

## Как добавить новость

1. Положи изображение JPG или PNG в `news/images`.
2. Открой `news/news.json`.
3. Добавь новый объект в начало массива `news`.
4. Укажи прямой raw-адрес фотографии.
5. Для видео укажи обычную ссылку YouTube, VK Видео или Rutube.
6. Сохрани изменения в GitHub.

Пример объекта:

```json
{
  "id": "update-0.4.0",
  "title": "Обновление 0.4.0",
  "date": "31.07.2026",
  "text": "Описание обновления.",
  "imageUrl": "https://raw.githubusercontent.com/Vadim-mim/roborust-updates/main/news/images/update-040.jpg",
  "videoUrl": "https://www.youtube.com/watch?v=YOUR_VIDEO_ID",
  "buttonText": "Смотреть трейлер"
}
```

Самую новую запись размещай первой. Пересобирать лаунчер после изменения `news.json` не требуется.

## Ограничения

- Используй JPG или PNG.
- Желательно не больше 2–3 МБ на одну фотографию.
- Не загружай большие MP4 в GitHub: лаунчер открывает видео по внешней ссылке.
- Лаунчер хранит последние новости и фотографии в `%LocalAppData%\RoboRustLauncher\NewsCache`.
