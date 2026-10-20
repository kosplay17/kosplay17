# Павел Родичев — IT Support и автоматизация поддержки

Работаю в технической поддержке и автоматизирую её: AI-бот первой линии, маршрутизация обращений,
инструменты для инженеров (Active Directory, Яндекс Tracker, киоски самообслуживания).
Здесь — сервисы, которые используются в работе, и учебные проекты.

## Содержание

* [Стек](#стек)
* [Сервисы](#сервисы)
* [Учебные проекты](#учебные-проекты)
* [Контакты](#контакты)

---

## Стек

* **Python:** FastAPI, Flask, ldap3, httpx, requests, pytest
* **LLM и поиск:** OpenAI-совместимые API, hybrid RAG (BM25 + embeddings), OCR
* **Интеграции:** Яндекс Tracker, Яндекс Wiki, Pachca, Active Directory (LDAPS)
* **Swift:** UIKit и WKWebView (iPadOS), Cocoa и WebKit (macOS, приложение в строке меню)
* **Инфраструктура:** Docker / Compose, macOS LaunchAgent, Git
* **Frontend:** JavaScript, React, Next.js, HTML / SCSS

---

## Сервисы

Рабочие инструменты IT Support:

| # | Название проекта | Описание проекта | Статус | Стек |
|:-:|---|---|:---:|---|
| 1 | [Support AI](https://github.com/kosplay17/support-ai-docs) | Корпоративный AI Service Desk. Принимает обращения в Pachca, находит инструкции в Яндекс Wiki (hybrid RAG), отвечает в треде с кнопками обратной связи и при необходимости создаёт тикет в Яндекс Tracker с автоматической маршрутизацией по системе, локации, очереди и категории. Admin UI без деплоя, аналитика CSAT / deflection / SLA, SLA-алерты исполнителям, OCR скриншотов, incident mode. *Код закрыт — по ссылке описание продукта и документация.* | используется, v2.0 | Python, FastAPI, LLM, RAG, Pachca, Яндекс Tracker, Яндекс Wiki, Docker |
| 2 | [VIP Support Bot](https://github.com/kosplay17/vip-support-bot) | Бот VIP-канала поддержки: каждое новое сообщение в Pachca превращается в задачу в Яндекс Tracker с автором-сотрудником, бот отвечает в треде ссылкой на задачу и упоминанием дежурных. Догон пропущенных сообщений, если вебхук не дошёл (без дублей), проверка подписи вебхука. | используется | Python, Flask, Pachca API, Yandex Tracker API, PythonAnywhere |
| 3 | [AD Console](https://github.com/kosplay17/ad-console) | Локальная веб-консоль Active Directory для macOS: поиск пользователей, компьютеров и групп, статус учётной записи, прямые и вложенные группы, разблокировка, сброс пароля, удаление из группы. Все операции — под учёткой оператора; CSRF, защита от DNS rebinding, лимит входа, журнал действий. Своё окно и иконка в строке меню на Swift. | используется | Python, FastAPI, ldap3, JavaScript, Swift |
| 4 | [Form Router](https://github.com/kosplay17/form-router) | Подбирает нужную форму обращения в IT Support по свободному описанию проблемы: сначала упорядоченные правила, при промахе — LLM через OpenAI-совместимый API с валидацией ответа. Каталог форм в JSON, лимит запросов, безопасный вывод на странице. | завершён | Python, FastAPI, httpx, LLM, JavaScript |
| 5 | [IT Support Kiosk](https://github.com/kosplay17/ipad-it-support-kiosk) | Приложение-киоск для iPad со страницей вики IT Support: белый список доменов, кнопка «Домой», возврат на главную после 30 секунд бездействия, автовход сервисной учётной записи (SSO / ADFS + TOTP) с хранением данных в Keychain, меню администратора по PIN. | используется | Swift, UIKit, WKWebView, XcodeGen |
| 6 | [Job Agent](https://github.com/kosplay17/job-agent) | Локальный агент поиска работы: hh.ru + карьерные сайты, двухфазный LLM-скоринг, оценка оклада, резюме и письмо под вакансию, отклик только после Approve (браузерная сессия соискателя). *Репозиторий приватный.* | в работе | Python, FastAPI, Playwright, SQLite, LLM |

---

## Учебные проекты

| # | Название проекта | Описание проекта | Статус | Стек |
|:-:|---|---|:---:|---|
| 1 | [react-pizza](https://github.com/kosplay17/react-pizza) | Вёрстка сайта с шаблонами EJS и сборкой на Gulp. | завершён | JavaScript, EJS, SCSS, Gulp, Bootstrap |
| 2 | [web](https://github.com/kosplay17/web) | Учебный проект на Next.js. | завершён | Next.js, React, TypeScript, CSS |
| 3 | [learn](https://github.com/kosplay17/learn) | Упражнения курса JavaScript (Udemy) и учебный сайт автосервиса на PHP + MySQL. | завершён | JavaScript, PHP, MySQL, HTML / CSS |

---

## Контакты

* **Telegram:** [@prodichev](https://t.me/prodichev)
* **GitHub:** [kosplay17](https://github.com/kosplay17)
