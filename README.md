# client-dev

Сайт-навчальний проєкт: **«Програмне забезпечення»**, кожна лабораторна — окремий коміт у `main`.

> **Поточний `main`:** останній коміт `2edefb9` — додано цей README.  
> Щоб чек-аутитись **рівно після Lab 8 (код без README)**, використовуйте `7b9d6f3`.

## Клонування

```bash
git clone https://github.com/DanyloDiachenko/client-dev.git
cd client-dev
```

Переконайтесь, що гілка оновлена:

```bash
git pull origin main
```

## Коміти (зручно чек-аутитись на будь-яку лабу)

Переглянути історію:

```bash
git log --oneline
```

| Lab | Hash (короткий) | Повідомлення коміту |
|-----|-----------------|----------------------|
| — | `f285135` | first lab (стартовий снапшот до Lab 1) |
| **1** | `a37a5e1` | Lab 1: базова верстка — чотири HTML-сторінки про програмне забезпечення |
| **2** | `379a377` | Lab 2: HTML — посилання, форматування, списки, таблиці, iframe, тема ПЗ |
| **3** | `5c9f5d7` | Lab 3: CSS — зовнішні/внутрішні стилі, пріоритет, оформлення списків і таблиць |
| **4** | `39eebad` | Lab 4: CSS-селектори — контекстні, дочірні, сусідні (.lab4-scope на about.html) |
| **5** | `a991701` | Lab 5: блокова верстка, float, position, псевдокласи та псевдоелементи (services.html) |
| **6** | `69fd932` | Lab 6: JavaScript — alert/prompt/confirm, зовнішній script.js, DOM, document.write, redirect.html |
| **7** | `5d76e0c` | Lab 7: події миші та клавіатури — делегування, data-action, events.js на index.html |
| **8** | `7b9d6f3` | Lab 8: події миші на contact.html — drag-and-drop, mouseover/out (mouse.js, mouse-demo.css) |

## Checkout на конкретну лабу

**Варіант A — від’єднаний HEAD (лише перегляд):**

```bash
git checkout 5c9f5d7
```

Повернутись на актуальний `main`:

```bash
git checkout main
git pull origin main
```

**Варіант B — окрема гілка від стану лаби (зручно для змін):**

```bash
git checkout -b lab-3-css 5c9f5d7
```

**Варіант C — повний hash (якщо потрібно однозначно):**

```bash
git rev-parse 7b9d6f3          # показати повний hash
git checkout <повний-hash>
```

Повний hash можна подивитися так:

```bash
git rev-parse 7b9d6f3
```

## Швидкий перехід між лабами

Наприклад, тільки Lab 1 або тільки після Lab 6:

```bash
git checkout a37a5e1    # стан після Lab 1
git checkout 69fd932    # стан після Lab 6
git checkout main       # останній коміт (за замовчуванням після Lab 8 — 7b9d6f3 у історії main)
```
