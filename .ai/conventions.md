# Code Conventions

## General Principles
<!-- Общие принципы написания кода в проекте -->
- [Принцип 1, например: Пишем читаемый код, а не умный]
- [Принцип 2, например: Явное лучше неявного]
- [Принцип 3]

## Naming Conventions

### Variables & Functions
- **Style:** [camelCase / snake_case / PascalCase]
- **Booleans:** [префикс is/has/should, например: is_active, has_permission]
- **Constants:** [UPPER_SNAKE_CASE]

**Examples:**
```[язык]
# Good
user_name = "John"
is_active = True

# Bad
un = "John"
active = True
```

### Files & Directories
- **Files:** [naming style, например: snake_case.py]
- **Directories:** [naming style, например: lowercase]
- **Test files:** [паттерн, например: test_*.py или *_test.py]

### Classes & Modules
- **Classes:** [PascalCase]
- **Private methods:** [префикс/суффикс, например: _private_method]

## Code Structure

### Imports
<!-- Порядок и стиль импортов -->
```[язык]
# 1. Стандартная библиотека
import os
import sys

# 2. Сторонние библиотеки
import requests
from fastapi import FastAPI

# 3. Локальные модули
from .models import User
from .utils import helper
```

### Function Length
- **Максимум:** [N строк, например: 50]
- **Если больше:** [разбить на подфункции]

### File Length
- **Максимум:** [N строк, например: 300-500]
- **Если больше:** [разбить на модули]

## Comments & Documentation

### When to Comment
- [Когда комментировать, например: Сложная бизнес-логика]
- [Когда НЕ комментировать, например: Очевидный код]

### Docstrings
```[язык]
def example_function(param1: str, param2: int) -> bool:
    """
    [Краткое описание что делает функция]
    
    Args:
        param1: [описание параметра]
        param2: [описание параметра]
    
    Returns:
        [описание возвращаемого значения]
    """
    pass
```

### Inline Comments
```[язык]
# Good: Объясняет WHY, а не WHAT
result = calculate_tax(amount)  # Используем упрощённую схему для MVP

# Bad: Объясняет очевидное
x = x + 1  # Увеличиваем x на 1
```

## Error Handling

### Exceptions
- **Используем:** [специфичные исключения, например: ValueError, не Exception]
- **Логирование:** [всегда логируем исключения]
- **Recovery:** [как обрабатываем ошибки]

**Example:**
```[язык]
try:
    result = dangerous_operation()
except SpecificError as e:
    logger.error(f"Operation failed: {e}")
    # Handle gracefully
```

## Testing Conventions

### Test Structure
- **Arrange-Act-Assert** pattern
- **One test = one assertion** [или несколько связанных]

### Test Naming
```[язык]
def test_[function_name]_[scenario]_[expected_result]():
    # Example: test_create_user_with_valid_data_returns_user()
    pass
```

## Git Conventions

### Commit Messages
```
[type]: [краткое описание]

[опциональное подробное описание]

Примеры типов:
- feat: новая функциональность
- fix: исправление бага
- docs: изменения в документации
- refactor: рефакторинг кода
- test: добавление тестов
```

### Branch Naming
- **Feature:** `feature/[название]`
- **Bugfix:** `bugfix/[название]`
- **Hotfix:** `hotfix/[название]`

## Code Style

### Formatting
- **Indentation:** [количество пробелов, например: 4 spaces]
- **Line length:** [максимум символов, например: 88 или 120]
- **Quotes:** [одинарные/двойные, например: double quotes]

### Linting & Formatting Tools
- **Linter:** [например: pylint, eslint, phpcs]
- **Formatter:** [например: black, prettier, php-cs-fixer]
- **Run before commit:** [yes/no]

## Database Conventions

### Table Names
- **Style:** [plural/singular, snake_case, например: users, order_items]

### Column Names
- **Style:** [snake_case]
- **Foreign keys:** [паттерн, например: user_id, order_id]
- **Timestamps:** [created_at, updated_at]

### Migrations
- **Naming:** [паттерн, например: YYYY_MM_DD_HHMMSS_description]
- **Never:** [не изменяем старые миграции]

## API Conventions (if applicable)

### Endpoint Naming
- **Style:** [kebab-case / snake_case]
- **Versioning:** [/api/v1/]
- **Resources:** [plural nouns, например: /users, /orders]

### HTTP Methods
- **GET:** получение данных
- **POST:** создание ресурса
- **PUT/PATCH:** обновление
- **DELETE:** удаление

### Response Format
```json
{
  "success": true,
  "data": {},
  "error": null
}
```

## Security Conventions

### Sensitive Data
- **Never:** [хардкодить пароли, ключи, токены]
- **Use:** [переменные окружения]
- **Store:** [в .env файле (не коммитить!)]

### Passwords
- **Always:** [хэшировать перед сохранением]
- **Never:** [логировать или показывать пароли]

## Project-Specific Conventions
<!-- Любые уникальные соглашения для этого проекта -->
- [Соглашение 1]
- [Соглашение 2]
