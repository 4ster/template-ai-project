# Template Roadmap

## Current Status

**Version:** 0.0.1  
**Date:** January 11, 2026  
**Status:** Alpha

## Completed Milestones

### v0.0.1 - Initial Release (January 2026)

**Core Structure:**
- ✅ `.ai/` directory with AI context files
  - project-overview.md
  - tech-stack.md
  - architecture.md
  - conventions.md
  - common-tasks.md
- ✅ Prompts library for common tasks
  - refactoring.md
  - debugging.md
  - documentation.md
- ✅ Product documentation template (docs/product.md)
- ✅ Backlog management (backlog.md)
- ✅ Developer documentation
  - README.md
  - CONTRIBUTING.md
- ✅ Configuration files
  - .editorconfig
  - .gitignore
- ✅ Template metadata
  - .template/USAGE.md with comprehensive usage guide
  - .template/ROADMAP.md

**Key Features:**
- Stack-agnostic base template
- Optimized for Claude integration
- Comprehensive documentation structure
- Ready-to-use AI prompts
- Product and business context support

---

## Upcoming Plans

### Next Release (v0.1.0) - Stack-Specific Templates

**Priority: High**

- [ ] **Python template**
  - requirements.txt / pyproject.toml
  - Docker Compose with PostgreSQL/Redis
  - pytest configuration
  - Python-specific conventions
  
- [ ] **JavaScript/TypeScript template**
  - package.json with common dependencies
  - Docker Compose with MongoDB/PostgreSQL
  - Jest/Vitest configuration
  - ESLint & Prettier configs
  
- [ ] **PHP template**
  - composer.json
  - Docker Compose with MySQL
  - PHPUnit configuration
  - PHP-CS-Fixer config

**Common additions for all stacks:**
- [ ] `.env.example` files
- [ ] Docker Compose templates
- [ ] Basic CI/CD templates (GitLab CI)

---

### Future Plans

### Integration with Other AI Tools

**Goal:** Make template compatible with multiple AI coding assistants

- [ ] `.cursorrules` file for Cursor IDE
- [ ] GitHub Copilot-specific instructions
- [ ] Comparison guide: when to use which tool
- [ ] Cross-tool prompt library
- [ ] AI tools configuration guide

### Testing Templates

**Goal:** Ready-to-use testing setup for different types of tests

- [ ] Unit testing templates
  - Setup and structure
  - Example tests
  - Mocking patterns
  
- [ ] Integration testing templates
  - Database setup
  - API testing examples
  - Test fixtures
  
- [ ] E2E testing templates
  - Selenium/Playwright setup
  - Common scenarios
  - CI integration

### CLI Tool for Template Setup

**Goal:** Automate template initialization and configuration

**Features:**
- [ ] Single command initialization
- [ ] Automatic placeholder replacement
- [ ] Stack detection and configuration
- [ ] Interactive setup wizard
- [ ] Pre-commit hooks installation

**Example usage:**
```bash
npx create-ai-project my-app --stack python
# or
ai-template init --interactive
```

### Interactive Wizard

**Goal:** Guide users through template customization

**Features:**
- [ ] Project type selection (web app, API, library, etc.)
- [ ] Stack selection (Python, JS, PHP, Go, etc.)
- [ ] Optional components selection
  - Database (PostgreSQL, MySQL, MongoDB)
  - Cache (Redis, Memcached)
  - Queue (Celery, Bull, RabbitMQ)
  - Frontend (React, Vue, none)
- [ ] AI tools preference
- [ ] Deployment target (Docker, Kubernetes, Serverless)
- [ ] Automatic file generation based on choices
- [ ] One-command project setup

**Example flow:**
```
? What type of project? › API
? Choose your stack › Python
? Database? › PostgreSQL
? Need caching? › Yes (Redis)
? AI tools? › Claude, Cursor
? Setup CI/CD? › GitLab CI
✓ Generating project structure...
✓ Installing dependencies...
✓ Project ready!
```

---

## Version History

### v0.0.1 (January 11, 2026)
- Initial alpha release
- Base template structure
- AI context framework
- Documentation templates
