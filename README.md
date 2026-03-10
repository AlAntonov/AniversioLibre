> 🌐 Jump to: [English](#-english) | [Русский](#-русский)

---

## 🇬🇧 English

# Aniversio Libre

> A minimalist parallel-text reader for the browser. Place your source and translation side by side — paragraph by paragraph.

---

## ✨ Features

- **Parallel reading** — source (`src.txt`) and translation (`trn.txt`) paragraphs are displayed in pairs, aligned one-to-one
- **Full-text search** — instantly highlights matches in both source and translation; navigate between results with `Enter` / `Shift+Enter`
- **Adjustable font size** — slider in the header, range 12–26 px
- **Dark / Light theme** — toggle with a single button; preference is saved in `localStorage`
- **Reading progress bar** — thin accent bar below the header shows how far you've scrolled
- **Active paragraph tracking** — the paragraph closest to the center of the viewport is highlighted automatically while scrolling
- **Keyboard navigation** — `↓` / `j` next paragraph, `↑` / `k` previous, `Ctrl+F` focus search, `Esc` clear search
- **Status bar** — shows total paragraph count, current position, and scroll percentage
- **Responsive layout** — works on mobile screens
- **Zero dependencies** — pure HTML + CSS + vanilla JS, no frameworks or build tools

---

## 🚀 Quick Start

1. Clone or download the repository.
2. Place your text files next to `index.html`:
   - `src.txt` — source text
   - `trn.txt` — translation
3. Start a local web server in the project folder:

```bash
python -m http.server
```

4. Open `http://localhost:8000` in your browser.

> **Why a server?** The page fetches `src.txt` and `trn.txt` via `fetch()`, which browsers block for `file://` URLs due to CORS policy.

Alternatively, use the **Live Server** extension in VS Code.

---

## 📁 File Format

- Plain UTF-8 text files (`.txt`)
- Paragraphs are separated by **one or more blank lines**
- The *n*-th paragraph of `src.txt` is paired with the *n*-th paragraph of `trn.txt`
- If one file has more paragraphs than the other, the extra paragraphs render with an empty counterpart

**Example `src.txt`:**
```
It was a bright cold day in April,
and the clocks were striking thirteen.

Winston Smith, his chin nuzzled into
his breast in an effort to escape the vile wind...
```

**Example `trn.txt`:**
```
Был холодный ясный апрельский день,
и часы пробили тринадцать.

Уинстон Смит, подбородок которого
был прижат к груди, спасаясь от злого ветра...
```

---

## ⌨️ Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `↓` or `j` | Next paragraph |
| `↑` or `k` | Previous paragraph |
| `Ctrl+F` / `Cmd+F` | Focus search field |
| `Enter` | Next search result |
| `Shift+Enter` | Previous search result |
| `Esc` | Clear search |

---

## 🛠️ Tech Stack

| | |
|---|---|
| **Markup** | HTML5 |
| **Styles** | CSS3 (custom properties, flexbox, sticky positioning) |
| **Logic** | Vanilla JavaScript (ES2017+, async/await) |
| **Font** | [Lora](https://fonts.google.com/specimen/Lora) via Google Fonts |

---

## 📄 License

Apache 2.0

---

---

## 🇷🇺 Русский

# Aniversio Libre

> Минималистичная читалка параллельных текстов для браузера. Оригинал и перевод — абзац за абзацем, рядом.

---

## ✨ Возможности

- **Параллельное чтение** — абзацы оригинала (`src.txt`) и перевода (`trn.txt`) отображаются парами, выровненными один к одному
- **Полнотекстовый поиск** — мгновенная подсветка совпадений в обоих текстах; навигация по результатам через `Enter` / `Shift+Enter`
- **Настройка размера шрифта** — ползунок в шапке, диапазон 12–26 пх
- **Тёмная / светлая тема** — переключение одной кнопкой; выбор сохраняется в `localStorage`
- **Полоса прогресса чтения** — тонкая акцентная линия под шапкой показывает, насколько прокручена страница
- **Отслеживание активного абзаца** — абзац, ближайший к центру экрана, подсвечивается автоматически при прокрутке
- **Клавиатурная навигация** — `↓` / `j` следующий абзац, `↑` / `k` предыдущий, `Ctrl+F` фокус на поиске, `Esc` сбросить поиск
- **Строка состояния** — показывает количество абзацев, текущую позицию и процент прокрутки
- **Адаптивный дизайн** — корректно работает на мобильных устройствах
- **Без зависимостей** — чистый HTML + CSS + ванильный JS, никаких фреймворков и сборщиков

---

## 🚀 Быстрый старт

1. Склонируйте или скачайте репозиторий.
2. Положите текстовые файлы рядом с `index.html`:
   - `src.txt` — исходный текст
   - `trn.txt` — перевод
3. Запустите локальный веб-сервер в папке проекта:

```bash
python -m http.server
```

4. Откройте `http://localhost:8000` в браузере.

> **Зачем сервер?** Страница загружает `src.txt` и `trn.txt` через `fetch()`, а браузеры блокируют такие запросы для `file://`-адресов из-за политики CORS.

Также можно использовать расширение **Live Server** в VS Code.

---

## 📁 Формат файлов

- Обычные текстовые файлы в кодировке UTF-8 (`.txt`)
- Абзацы разделяются **одной или несколькими пустыми строками**
- *n*-й абзац `src.txt` ставится в пару с *n*-м абзацем `trn.txt`
- Если в одном файле абзацев больше, лишние отображаются с пустым «двойником»

**Пример `src.txt`:**
```
It was a bright cold day in April,
and the clocks were striking thirteen.

Winston Smith, his chin nuzzled into
his breast in an effort to escape the vile wind...
```

**Пример `trn.txt`:**
```
Был холодный ясный апрельский день,
и часы пробили тринадцать.

Уинстон Смит, подбородок которого
был прижат к груди, спасаясь от злого ветра...
```

---

## ⌨️ Горячие клавиши

| Клавиша | Действие |
|---------|----------|
| `↓` или `j` | Следующий абзац |
| `↑` или `k` | Предыдущий абзац |
| `Ctrl+F` / `Cmd+F` | Фокус на строке поиска |
| `Enter` | Следующий результат поиска |
| `Shift+Enter` | Предыдущий результат поиска |
| `Esc` | Сбросить поиск |

---

## 🛠️ Стек технологий

| | |
|---|---|
| **Разметка** | HTML5 |
| **Стили** | CSS3 (флексбокс, sticky-позиционирование) |
| **Логика** | Ванильный JavaScript (ES2017+, async/await) |
| **Шрифт** | [Lora](https://fonts.google.com/specimen/Lora) через Google Fonts |

---

## 📄 Лицензия

Apache 2.0
