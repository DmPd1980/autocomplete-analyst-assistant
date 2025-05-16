# Autocomplete Analyst Assistant

🔠 Интеллектуальный помощник системного аналитика, помогающий формировать требования, управлять глоссарием и использовать базу знаний с RAG (Retrieval-Augmented Generation).

## 🚀 Возможности

* Режимы генерации требований (Use Case, User Story и др.)
* Глоссарий терминов с возможностью редактирования
* История сгенерированных требований
* Интеграция с RAG (ChromaDB + SentenceTransformers)
* Загрузка пользовательских документов (.docx, .pdf)
* Дерево требований и экспорт в JSON
* Веб-интерфейс (HTML + JavaScript)
* Локальный запуск без интернета

## 💠 Установка

### 1. Клонируй репозиторий

```bash
git clone https://github.com/DmPd1980/autocomplete-analyst-assistant.git
cd autocomplete-analyst-assistant
```

### 2. Установи зависимости

```bash
npm install
```

### 3. Убедись, что установлен [Ollama](https://ollama.com/) и запущена модель (например, Mistral):

```bash
ollama run mistral
```

### 4. Запусти сервер

```bash
node server.js
```

Открой браузер: [http://localhost:3000](http://localhost:3000)

---

## 📂 Структура проекта

```
autocomplete-analyst-assistant/
├── public/             # Интерфейс (HTML, CSS, JS)
├── routes/             # API-роуты (история, режимы, генерация)
├── utils/              # Промпты и режимы генерации
├── rag-engine/         # RAG: ChromaDB + ingest + поиск
│   └── docs/           # Загружаемые документы
├── chroma/             # Векторная база знаний (chroma.sqlite3)
├── tree.json           # Сохранённое дерево требований
├── package.json        # Зависимости проекта
└── server.js           # Основной сервер
```

---

## 📌 Заметки

* ✅ Минимальные требования: Node.js, Ollama, Python + venv (для RAG)
* ✅ Поддержка RAG включается через чекбокс в интерфейсе
* 🔪 Поддержка сравнения генерации с RAG и без него

---

## 📌 Лицензия

MIT License. Используй, улучшай и делись!
