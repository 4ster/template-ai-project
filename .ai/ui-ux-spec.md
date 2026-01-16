# UI/UX Specification

## Design Principles

### Core Principles
<!-- Основные принципы дизайна проекта -->
1. **[Принцип 1]** — [описание, например: Touch-First — интерфейс оптимизирован для сенсорного управления]
2. **[Принцип 2]** — [описание, например: Instant Feedback — каждое действие даёт визуальный отклик]
3. **[Принцип 3]** — [описание, например: Minimal Friction — минимум подтверждений, максимум скорости работы]
4. **[Принцип 4]** — [описание, например: Responsive & Adaptive — от 320px до 4K экранов]
5. **[Принцип 5]** — [описание, например: Accessibility — контрастность минимум 4.5:1]

### Visual Language
<!-- Визуальный язык дизайна -->
- **Typography:** [шрифты, например: SF Pro / Roboto / System fonts]
- **Color Palette:**
  ```
  Primary Background:   #[цвет]
  Secondary Background: #[цвет]
  Accent:               #[цвет]
  Success:              #[цвет]
  Warning:              #[цвет]
  Error:                #[цвет]
  Text Primary:         #[цвет]
  Text Secondary:       #[цвет]
  ```
- **Spacing Scale:** [размеры, например: 4px, 8px, 12px, 16px, 20px, 24px, 32px, 40px]
- **Border Radius:** [размеры, например: 8px (small), 12px (medium), 20px (large)]
- **Shadows:** [описание теней]

---

## Screen Specifications

### 1. [Название экрана] (`/route`)

**Назначение:** [Что делает этот экран]

**Layout:**
```
┌─────────────────────────────────────┐
│          [Header]                   │
├─────────────────────────────────────┤
│                                     │
│  [Основной контент]                 │
│                                     │
├─────────────────────────────────────┤
│  [Footer / Actions]                 │
└─────────────────────────────────────┘
```

**Components:**
- **[Компонент 1]** — [описание и поведение]
- **[Компонент 2]** — [описание и поведение]

**States:**
- Empty state: [описание]
- Loading: [описание]
- Error: [описание]
- Success: [описание]

---

### 2. [Следующий экран] (`/route`)

<!-- Повторить структуру для каждого экрана -->

---

## Modals & Dialogs

### Confirmation Dialog (Template)
```
┌─────────────────────────────────────┐
│         [Icon]                      │
│                                     │
│  [Title]                            │
│                                     │
│  [Description text]                 │
│                                     │
│  [Secondary Button] [Primary Button]│
└─────────────────────────────────────┘
```

**Styling:**
- Background: [описание]
- Modal: [описание]
- Max-width: [размер]
- Padding: [размер]
- Buttons: [описание]

### Common Modals:

#### [Название модалки]
```
┌───────────────────────────┐
│       [Icon]              │
│ [Title]                   │
│                           │
│ [Content]                 │
│                           │
│ [Cancel] [Confirm]        │
└───────────────────────────┘
```

---

## Toasts & Notifications

**Position:** [позиция на экране]
**Duration:** [длительность]
**Styling:** [описание стиля]

**Types:**

1. **Success**
   - Background: [цвет]
   - Icon: [иконка]

2. **Error**
   - Background: [цвет]
   - Icon: [иконка]

3. **Info**
   - Background: [цвет]
   - Icon: [иконка]

4. **Warning**
   - Background: [цвет]
   - Icon: [иконка]

**Examples:**
- "[Пример сообщения 1]"
- "[Пример сообщения 2]"

---

## Loading States

### Skeleton Screens
<!-- Описание skeleton-загрузчиков -->

```
┌─────────────────────────────────────┐
│ ████████ vs ████████               │
│ ████ • ███ • ████                  │
│ [██████] [█████]                   │
└─────────────────────────────────────┘
```

**Animation:**
```css
@keyframes skeleton-pulse {
  0%, 100% { opacity: 0.4; }
  50% { opacity: 0.7; }
}
```

### Spinners
<!-- Описание спиннеров -->

---

## Empty States

### [Название пустого состояния]
```
┌─────────────────────────────────────┐
│              [Icon]                 │
│                                     │
│      [Заголовок]                    │
│                                     │
│   [Описание]                        │
│                                     │
│      [CTA Button]                   │
└─────────────────────────────────────┘
```

---

## Interactive Elements

### Gestures (if applicable)
<!-- Описание жестов для touch-интерфейсов -->

1. **[Жест 1, например: Swipe Up/Down]**
   - **Action:** [действие]
   - **Feedback:** [обратная связь]
   - **Threshold:** [минимальная дистанция]

2. **[Жест 2, например: Long Press]**
   - **Action:** [действие]
   - **Duration:** [время активации]
   - **Feedback:** [обратная связь]

### Keyboard Shortcuts (if applicable)
<!-- Горячие клавиши для desktop -->
- `[Клавиша]` — [действие]
- `[Клавиша]` — [действие]

---

## Responsive Design

### Breakpoints
```css
/* Mobile S */
@media (max-width: 374px) { }

/* Mobile M */
@media (min-width: 375px) and (max-width: 767px) { }

/* Tablet */
@media (min-width: 768px) and (max-width: 1023px) { }

/* Desktop */
@media (min-width: 1024px) { }

/* Large screens */
@media (min-width: 1440px) { }
```

### Touch Target Sizes
- Minimum: [размер, например: 44x44px]
- Recommended: [размер, например: 48x48px]
- Spacing between targets: [размер]

### Font Scaling
```css
/* Mobile */
@media (max-width: 767px) {
  h1 { font-size: [размер]; }
  body { font-size: [размер]; }
}

/* Desktop */
@media (min-width: 1024px) {
  h1 { font-size: [размер]; }
  body { font-size: [размер]; }
}
```

---

## Accessibility (a11y)

### Semantic HTML
```html
<header role="banner">
<nav role="navigation" aria-label="Main">
<main role="main">
<button aria-label="[описание действия]">
```

### Keyboard Navigation
- Tab order: [описание порядка]
- Focus indicators: [описание]
- Shortcuts: [список горячих клавиш]

### Screen Readers
- ARIA labels на интерактивных элементах
- Live regions для динамических обновлений
- Alt text на изображениях

### Color Contrast
- Текст на фоне: минимум [ratio, например: 4.5:1] (WCAG AA)
- Крупный текст: минимум [ratio, например: 3:1]

---

## Animation Guidelines

### Timing Functions
```css
--ease-in-out: cubic-bezier(0.4, 0, 0.2, 1);
--ease-out: cubic-bezier(0, 0, 0.2, 1);
--ease-in: cubic-bezier(0.4, 0, 1, 1);
```

### Duration Scale
- **Fast (100-200ms):** [использование]
- **Medium (200-400ms):** [использование]
- **Slow (400-600ms):** [использование]

### Key Animations
<!-- Описание ключевых анимаций -->

```css
@keyframes [animation-name] {
  0% { /* начальное состояние */ }
  100% { /* конечное состояние */ }
}
```

### Reduced Motion
```css
@media (prefers-reduced-motion: reduce) {
  * {
    animation-duration: 0.01ms !important;
    transition-duration: 0.01ms !important;
  }
}
```

---

## Error States

### [Тип ошибки 1, например: Offline Mode]
```
┌─────────────────────────────────────┐
│ ⚠️ [Заголовок]                      │
│                                     │
│ [Описание проблемы]                 │
│ [Что делать пользователю]           │
└─────────────────────────────────────┘
```

### [Тип ошибки 2, например: 404 Not Found]
<!-- Описание -->

### [Тип ошибки 3, например: Server Error]
<!-- Описание -->

---

## Component Library

### Button Variants
```jsx
// Primary
<Button variant="primary">[Текст]</Button>

// Secondary
<Button variant="secondary">[Текст]</Button>

// Ghost
<Button variant="ghost">[Текст]</Button>

// Danger
<Button variant="danger">[Текст]</Button>
```

### Input Fields
```jsx
<Input
  label="[Label]"
  placeholder="[Placeholder]"
  error="[Error message]"
/>
```

### Badges
```jsx
<Badge variant="[variant]">[Text]</Badge>
```

### Cards
```jsx
<Card>
  <CardHeader>
    <CardTitle>[Title]</CardTitle>
  </CardHeader>
  <CardContent>
    {/* Content */}
  </CardContent>
  <CardActions>
    <Button>[Action]</Button>
  </CardActions>
</Card>
```

---

## Performance Budgets

### Bundle Size
- Initial JS: < [размер] (gzipped)
- CSS: < [размер] (gzipped)
- Fonts: < [размер]

### Metrics
- First Contentful Paint (FCP): < [время]
- Largest Contentful Paint (LCP): < [время]
- Time to Interactive (TTI): < [время]
- Cumulative Layout Shift (CLS): < [значение]

### Image Optimization
- [Рекомендации по оптимизации изображений]

---

## Internationalization (i18n)

<!-- Если применимо -->
```javascript
const translations = {
  ru: {
    '[key]': '[перевод]',
  },
  en: {
    '[key]': '[translation]',
  },
};
```

---

## Print Styles (if applicable)

```css
@media print {
  /* Скрыть элементы интерфейса */
  nav, button, .controls { display: none; }

  /* Оптимизировать для печати */
  body {
    background: white;
    color: black;
  }
}
```

---

## Notes for Implementation

<!-- Любые дополнительные заметки для разработчиков -->
- [Заметка 1]
- [Заметка 2]
- [Заметка 3]
