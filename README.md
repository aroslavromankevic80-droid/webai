```markdown
# ⚡ WebAI 1.0.4 Поддержка:https://forms.gle/bB9Y86eLBKghmqFAA

Универсальный, лёгкий и полностью автономный веб-клиент для работы с любыми LLM через API в одном HTML-файле. Не требует установки Node.js или сервера — достаточно просто открыть файл в браузере.

---

## ✨ Возможности

- 🔌 **Поддержка любых провайдеров**: Tooken Club, xAI (Grok), OpenAI, OpenRouter, Google Gemini, DeepSeek, Groq, Ollama (локально).
- ⌨️ **Удобный ввод**: отправка строго по **Enter**, перевод строки — **Shift + Enter**.
- 🖼 **Мультимодальность**: вставка скриншотов прямо из буфера обмена (`Ctrl + V`) и прикрепление файлов через скрепку.
- ⏹ **Управление генерацией**: возможность прервать ответ модели в реальном времени кнопкой «Стоп».
- 📊 **Контроль расходов**: точный подсчёт токенов за каждое сообщение и за весь диалог с оценкой стоимости.
- 📋 **Работа с кодом**: блоки кода с горизонтальным скроллом в одну строку, кнопками быстрого копирования и скачивания файла.
- 📄 **Экспорт**: сохранение переписки в чистый PDF-документ.
- 🌐 **Двуязычный интерфейс**: поддержка русского и 100% английского языка.

---

## 🚀 Быстрый старт

1. Перейдите в раздел [Releases](https://github.com/aroslavromankevic80-droid/webai/releases) и скачайте `index.html`[cite: 5].
2. Откройте скачанный файл двойным кликом в браузере.
3. Введите ваш API-ключ в верхней панели и начните общение!

---

## 🌐 Обход CORS (запуск в отдельном окне)

Некоторые сторонние сервисы (например, Tooken Club) не отдают браузерные заголовки CORS, из-за чего запросы из локального файла блокируются. 

> ⚠️ **Важно:** В обычном окне Chrome флаг безопасности не сработает из-за системной защиты браузера. Обязательно запускайте команду ниже — она создаст **новое отдельное окно разработки**, где CORS отключён на 100%.

### 🍏 macOS
Откройте **Терминал** и выполните:
```bash
open -na "Google Chrome" --args --user-data-dir="/tmp/chrome_cors_dev" --disable-web-security --disable-site-isolation-trials

```

### 🪟 Windows

Нажмите сочетание клавиш **Win + R**, вставьте команду и нажмите **Enter**:

```cmd
chrome.exe --user-data-dir="%LOCALAPPDATA%\Google\Chrome_Dev" --disable-web-security --disable-site-isolation-trials

```

*(Если не находит `chrome.exe`, используйте полный путь)*:

```cmd
"C:\Program Files\Google\Chrome\Application\chrome.exe" --user-data-dir="%LOCALAPPDATA%\Google\Chrome_Dev" --disable-web-security --disable-site-isolation-trials

```

### 🐧 Linux

Выполните в терминале:

```bash
google-chrome --user-data-dir="/tmp/chrome_cors_dev" --disable-web-security --disable-site-isolation-trials

```

*(Для Chromium)*:

```bash
chromium-browser --user-data-dir="/tmp/chrome_cors_dev" --disable-web-security --disable-site-isolation-trials

```

```

```
