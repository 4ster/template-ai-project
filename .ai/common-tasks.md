# Common Tasks

## Setting Up Development Environment

### First-time Setup
```bash
# 1. Клонировать репозиторий
git clone [URL]
cd [project-name]

# 2. [Установить зависимости]
[команда установки зависимостей]

# 3. [Настроить переменные окружения]
cp .env.example .env
# Отредактировать .env

# 4. [Запустить БД / сервисы]
docker-compose up -d

# 5. [Применить миграции]
[команда миграций]

# 6. [Запустить проект]
[команда запуска]
```

### Daily Startup
```bash
# Запустить зависимости
docker-compose up -d

# Запустить проект
[команда запуска]
```

## Working with Code

### Creating a New Feature
1. Создать ветку: `git checkout -b feature/[название]`
2. [Шаги разработки специфичные для проекта]
3. Написать тесты
4. Запустить тесты: `[команда]`
5. Закоммитить: `git commit -m "feat: [описание]"`
6. Отправить: `git push origin feature/[название]`

### Adding a New [Component/Module/Endpoint]
<!-- Пример для API: Adding a New Endpoint -->
1. Создать модель в `[путь]/models/`
2. Создать схему в `[путь]/schemas/`
3. Создать роут/контроллер в `[путь]/routes/`
4. Добавить бизнес-логику в `[путь]/services/`
5. Написать тесты в `tests/`
6. Обновить документацию

**Template:**
```[язык]
# [Пример кода для нового компонента]
```

### Refactoring Existing Code
1. Убедиться, что есть тесты для рефакторимого кода
2. Запустить тесты: `[команда]`
3. Провести рефакторинг
4. Запустить тесты снова — они должны проходить
5. Code review (если работаешь в команде)

## Testing

### Running All Tests
```bash
[команда запуска всех тестов]
```

### Running Specific Test
```bash
[команда запуска конкретного теста]
```

### Running Tests with Coverage
```bash
[команда запуска с coverage]
```

### Writing a New Test
```[язык]
# Template для нового теста
def test_[function]_[scenario]_[expected]():
    # Arrange
    [подготовка данных]
    
    # Act
    result = [вызов функции]
    
    # Assert
    assert result == [ожидаемый результат]
```

## Database Operations

### Creating a Migration
```bash
[команда создания миграции]
```

### Running Migrations
```bash
# Apply migrations
[команда применения миграций]

# Rollback
[команда отката миграций]
```

### Accessing Database Console
```bash
[команда доступа к БД]
```

### Seeding Test Data
```bash
[команда для наполнения тестовыми данными]
```

## Debugging

### Common Issues

#### [Проблема 1]
**Симптомы:** [описание]  
**Решение:**
```bash
[команды для решения]
```

#### [Проблема 2]
**Симптомы:** [описание]  
**Решение:**
```bash
[команды для решения]
```

### Logging
```[язык]
# Добавить логирование
import logging

logger = logging.getLogger(__name__)
logger.debug("Debug message")
logger.info("Info message")
logger.error("Error message")
```

### Debugging Tools
- **[Инструмент 1]:** [как использовать]
- **[Инструмент 2]:** [как использовать]

## Code Quality

### Running Linter
```bash
[команда запуска линтера]
```

### Auto-formatting Code
```bash
[команда форматирования]
```

### Type Checking (if applicable)
```bash
[команда проверки типов]
```

## Dependencies Management

### Adding a New Dependency
```bash
# Install
[команда установки пакета]

# Update dependency file
[как обновить requirements.txt / package.json / composer.json]
```

### Updating Dependencies
```bash
# Update all
[команда обновления]

# Update specific package
[команда обновления конкретного пакета]
```

### Checking for Outdated Dependencies
```bash
[команда проверки устаревших зависимостей]
```

## Git Workflows

### Creating a Feature Branch
```bash
git checkout -b feature/[название-фичи]
```

### Updating from Main Branch
```bash
git checkout main
git pull origin main
git checkout feature/[название]
git merge main
# Resolve conflicts if any
```

### Committing Changes
```bash
git add .
git commit -m "[type]: [краткое описание]"
```

### Before Pushing
```bash
# Run tests
[команда тестов]

# Run linter
[команда линтера]

# If all good
git push origin [branch-name]
```

## Performance Optimization

### Profiling Code
```bash
[команда профилирования]
```

### Finding Slow Database Queries
```bash
[как найти медленные запросы]
```

### Caching
```[язык]
# Example кэширования
[пример кода]
```

## Documentation

### Updating API Documentation
[Где находится и как обновлять документацию API]

### Generating Documentation
```bash
[команда генерации документации]
```

## Useful Commands Reference

```bash
# [Описание команды 1]
[команда]

# [Описание команды 2]
[команда]

# [Описание команды 3]
[команда]
```

## Getting Help

### Where to Look
1. [Документация проекта в docs/]
2. [README.md для быстрого старта]
3. [Backlog.md для текущих задач и известных проблем]
4. [Код — ищи похожие примеры в проекте]

### Asking for Help
- Опиши проблему подробно
- Приложи логи ошибок
- Укажи, что уже пробовал
