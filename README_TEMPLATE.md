# [Project Name]

> [Краткое описание проекта в одном предложении]

## Overview

[2-3 предложения о том, что делает проект, какую проблему решает, для кого предназначен]

## AI Context

> **Для AI-агентов:** Полный контекст проекта находится в директории `.ai/`
> - Начни с [.ai/project-overview.md](.ai/project-overview.md)
> - Технологии: [.ai/tech-stack.md](.ai/tech-stack.md)
> - Архитектура: [.ai/architecture.md](.ai/architecture.md)
> - Соглашения: [.ai/conventions.md](.ai/conventions.md)
> - UI/UX: [.ai/ui-ux-spec.md](.ai/ui-ux-spec.md)
> - User Stories: [.ai/user-stories.md](.ai/user-stories.md)
> - Частые задачи: [.ai/common-tasks.md](.ai/common-tasks.md)

## Tech Stack

- **Backend:** [язык, фреймворк]
- **Database:** [БД]
- **Frontend:** [если есть]
- **Infrastructure:** [Docker, Docker Compose, etc.]

См. подробности: [.ai/tech-stack.md](.ai/tech-stack.md)

## Features

- [Ключевая фича 1]
- [Ключевая фича 2]
- [Ключевая фича 3]

## Setup

### Prerequisites

- [Требование 1, например: Python 3.11+]
- [Требование 2, например: Docker & Docker Compose]
- [Требование 3, например: PostgreSQL 15+]

### Installation

```bash
# 1. Клонировать репозиторий
git clone [URL]
cd [project-name]

# 2. Установить зависимости
[команда установки, например: pip install -r requirements.txt]

# 3. Скопировать и настроить переменные окружения
cp .env.example .env
# Отредактируй .env файл

# 4. Запустить сервисы (БД и т.д.)
docker-compose up -d

# 5. Применить миграции
[команда миграций, например: alembic upgrade head]

# 6. Запустить проект
[команда запуска, например: python main.py]
```

### Quick Start

```bash
# Ежедневный запуск
docker-compose up -d
[команда запуска проекта]
```

Приложение будет доступно по адресу: `http://localhost:[PORT]`

## Testing

```bash
# Запустить все тесты
[команда тестов, например: pytest]

# Запустить с coverage
[команда с coverage, например: pytest --cov]
```

## Project Structure

```
project/
├── .ai/                        # AI контекст для агентов
│   ├── project-overview.md     # Краткий обзор проекта + ссылки
│   ├── architecture.md         # Техническая архитектура
│   ├── tech-stack.md           # Технологический стек
│   ├── conventions.md          # Соглашения по коду и стилю
│   ├── common-tasks.md         # Частые команды разработки
│   ├── ui-ux-spec.md           # Спецификация UI/UX дизайна
│   ├── user-stories.md         # Пользовательские истории
│   └── prompts/                # Готовые промпты для AI
│       ├── debugging.md        # Промпт для отладки
│       ├── documentation.md    # Промпт для документации
│       └── refactoring.md      # Промпт для рефакторинга
├── .claude/                    # Конфигурация Claude Code
├── docs/                       # Документация проекта
│   └── product.md              # Продуктовая информация
├── [src/app/etc]/              # Исходный код (твоя структура)
├── tests/                      # Тесты
├── .editorconfig               # Настройки редактора
├── .gitignore                  # Исключения для Git
├── AGENTS.md                   # Инструкции для AI-агентов (Copilot, Cursor и др.)
├── CLAUDE.md                   # Инструкции для Claude Code
├── CONTRIBUTING.md             # Гайд для контрибьюторов
├── backlog.md                  # Задачи и планы развития
└── README.md                   # Этот файл
```

## Contributing

См. [CONTRIBUTING.md](CONTRIBUTING.md) для деталей о процессе разработки.

### Quick Guidelines

- Следуй соглашениям из [.ai/conventions.md](.ai/conventions.md)
- Пиши тесты для новой функциональности
- Обновляй документацию при необходимости
- Используй осмысленные commit messages

## Development

### Common Tasks

См. полный список: [.ai/common-tasks.md](.ai/common-tasks.md)

**Частые команды:**
```bash
# Запустить линтер
[команда линтера]

# Форматировать код
[команда форматера]

# Создать миграцию
[команда миграции]
```

## Documentation

- **Product:** [docs/product.md](docs/product.md) - бизнес-контекст, пользователи, метрики
- **Architecture:** [.ai/architecture.md](.ai/architecture.md) - техническая архитектура
- **API:** [ссылка на API docs если есть]

## Roadmap

См. актуальный roadmap в [backlog.md](backlog.md)

## License

[Тип лицензии, например: MIT]

## Contact

- **Maintainer:** [Имя]
- **Email:** [email]
- **Issues:** [ссылка на issues]
