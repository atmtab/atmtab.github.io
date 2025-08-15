# IT Park Smart Search

Умный поиск резидентов IT-Park с использованием AI API DeepSeek.

## 🚀 Демо

[Открыть приложение](https://atmtab.github.io/)

## 🧪 Тестирование API

[Тест API DeepSeek](https://atmtab.github.io/test.html)

## 📁 Структура проекта

```
├── public/                 # Статические файлы для веб-приложения
│   ├── index.html         # Основное приложение
│   ├── styles.css         # Стили
│   ├── script.js          # Основная логика
│   ├── api.js             # Интеграция с DeepSeek API
│   └── test.html          # Тестирование API
├── data/                   # Данные компаний
│   ├── data.json          # Полные данные
│   └── data-mini.json     # Мини-данные для API
├── scripts/                # Скрипты сборки
│   └── build-gh-pages.js  # Сборка для GitHub Pages
├── .github/                # GitHub Actions
│   └── workflows/          # Workflow для деплоя
├── server.js               # Node.js сервер для разработки
├── package.json            # Зависимости и скрипты
└── README.md               # Документация
```

## 🚀 Быстрый старт

### Локальная разработка

```bash
# Установка зависимостей
npm install

# Запуск сервера разработки
npm run dev

# Открыть http://localhost:3000
```

### Сборка для GitHub Pages

```bash
# Сборка проекта
npm run build

# Предварительный просмотр
npm run preview

# Открыть http://localhost:8000
```

## 🔧 Технологии

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **AI API**: DeepSeek AI
- **Backend**: Node.js, Express.js (для разработки)
- **Deploy**: GitHub Pages, GitHub Actions

## 📝 Функциональность

- 🔍 Умный поиск компаний с помощью AI
- 🏢 База данных резидентов IT-Park
- 🤖 Интеграция с DeepSeek API
- 📱 Адаптивный дизайн
- 🔄 Fallback поиск при недоступности API
- 🧪 Тестирование API

## 🚀 Деплой

Проект автоматически деплоится на GitHub Pages при пуше в ветку `main`.

### Ручной деплой

1. Соберите проект: `npm run build`
2. Скопируйте содержимое папки `dist/` в ветку `gh-pages`
3. Или используйте GitHub Actions: `Actions` → `Deploy to GitHub Pages` → `Run workflow`

## 📊 API Endpoints

- `GET /api/companies` - полные данные компаний
- `GET /api/companies-mini` - мини-данные для API
- `POST /api/search` - поиск компаний
- `POST /api/test-deepseek` - тест DeepSeek API

## 🔑 Конфигурация

API ключ DeepSeek настраивается в файле `public/api.js`:

```javascript
constructor(apiKey = 'your-api-key-here') {
  this.apiKey = apiKey;
  // ...
}
```

## 📝 Лицензия

MIT License

## 🤝 Вклад в проект

1. Форкните репозиторий
2. Создайте ветку для новой функции
3. Внесите изменения
4. Создайте Pull Request

## 📞 Поддержка

По вопросам обращайтесь к команде IT-Park или создавайте Issues в репозитории.
