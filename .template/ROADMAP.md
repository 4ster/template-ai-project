# Template Roadmap

## Current Status

**Version:** 0.0.1
**Date:** 11 января 2026
**Status:** Alpha

## Completed Milestones

### v0.0.1 - Initial Release (January 2026)

**Core Structure:**
- ✅ Директория `.ai/` с AI-контекстом
  - project-overview.md
  - tech-stack.md
  - architecture.md
  - conventions.md
  - common-tasks.md
- ✅ Библиотека промптов для типовых задач
  - refactoring.md
  - debugging.md
  - documentation.md
- ✅ Шаблон продуктовой документации (docs/product.md)
- ✅ Управление бэклогом (backlog.md)
- ✅ Документация для разработчиков
  - README.md
  - CONTRIBUTING.md
- ✅ Конфигурационные файлы
  - .editorconfig
  - .gitignore
- ✅ Метаданные шаблона
  - .template/USAGE.md с подробной инструкцией
  - .template/ROADMAP.md

**Key Features:**
- Базовый шаблон, независимый от стека
- Оптимизирован для интеграции с Claude
- Продуманная структура документации
- Готовые промпты для AI
- Поддержка продуктового и бизнес-контекста

---

## Upcoming Plans

### Next Release (v0.1.0) - Stack-Specific Templates

**Priority: High**

- [ ] **Python template**
  - requirements.txt / pyproject.toml
  - Docker Compose с PostgreSQL/Redis
  - Конфигурация pytest
  - Python-специфичные соглашения

- [ ] **JavaScript/TypeScript template**
  - package.json с типовыми зависимостями
  - Docker Compose с MongoDB/PostgreSQL
  - Конфигурация Jest/Vitest
  - Конфиги ESLint & Prettier

- [ ] **PHP template**
  - composer.json
  - Docker Compose с MySQL
  - Конфигурация PHPUnit
  - Конфиг PHP-CS-Fixer

**Common additions for all stacks:**
- [ ] Файлы `.env.example`
- [ ] Шаблоны Docker Compose
- [ ] Базовые шаблоны CI/CD (GitLab CI)

---

### Future Plans

### Integration with Other AI Tools

**Goal:** Сделать шаблон совместимым с разными AI-ассистентами для кода

- [ ] Файл `.cursorrules` для Cursor IDE
- [ ] Инструкции для GitHub Copilot
- [ ] Гайд по сравнению: когда какой инструмент использовать
- [ ] Кросс-платформенная библиотека промптов
- [ ] Гайд по настройке AI-инструментов

### Testing Templates

**Goal:** Готовые конфигурации тестирования для разных типов тестов

- [ ] Шаблоны unit-тестов
  - Настройка и структура
  - Примеры тестов
  - Паттерны мокирования

- [ ] Шаблоны интеграционных тестов
  - Настройка базы данных
  - Примеры тестирования API
  - Тестовые фикстуры

- [ ] Шаблоны E2E-тестов
  - Настройка Selenium/Playwright
  - Типовые сценарии
  - Интеграция с CI

### CLI Tool for Template Setup

**Goal:** Автоматизация инициализации и настройки шаблона

**Features:**
- [ ] Инициализация одной командой
- [ ] Автоматическая замена плейсхолдеров
- [ ] Определение стека и настройка
- [ ] Интерактивный мастер настройки
- [ ] Установка pre-commit хуков

**Example usage:**
```bash
npx create-ai-project my-app --stack python
# или
ai-template init --interactive
```

### Interactive Wizard

**Goal:** Провести пользователя через кастомизацию шаблона

**Features:**
- [ ] Выбор типа проекта (веб-приложение, API, библиотека и т.д.)
- [ ] Выбор стека (Python, JS, PHP, Go и т.д.)
- [ ] Выбор опциональных компонентов
  - База данных (PostgreSQL, MySQL, MongoDB)
  - Кэш (Redis, Memcached)
  - Очереди (Celery, Bull, RabbitMQ)
  - Фронтенд (React, Vue, без фронтенда)
- [ ] Предпочтения по AI-инструментам
- [ ] Целевая платформа деплоя (Docker, Kubernetes, Serverless)
- [ ] Автоматическая генерация файлов на основе выбора
- [ ] Настройка проекта одной командой

**Example flow:**
```
? Тип проекта? › API
? Выбери стек › Python
? База данных? › PostgreSQL
? Нужен кэш? › Да (Redis)
? AI-инструменты? › Claude, Cursor
? Настроить CI/CD? › GitLab CI
✓ Генерация структуры проекта...
✓ Установка зависимостей...
✓ Проект готов!
```

---

## Version History

### v0.0.1 (11 января 2026)
- Первый альфа-релиз
- Базовая структура шаблона
- Фреймворк AI-контекста
- Шаблоны документации
