---
тип: документация
дата: 2026-10-02
для: реализация
---

# Minimal Theme Setup для дашборда

## Установка

1. Settings → Appearance → Theme → выбрать "Minimal"
2. Установить плагин **Minimal Theme Settings**
3. Settings → Minimal Theme Settings — откроется панель настроек

## CSS-классы для карточек

В frontmatter главной заметки добавить:

```yaml
cssclasses:
  - cards
  - cards-cols-3
  - hide-properties
```

Это автоматически стилизирует содержимое как карточки в 3 колонки.

## Кастомизация цветов (через Style Settings)

1. Установить плагин **Style Settings**
2. Settings → Style Settings (появится новая панель)
3. Найти секцию Minimal Theme
4. Настроить:
   - Accent color: `#d4fb72` (лайм)
   - Background: `#101515` (темный)
   - Text color: `#f2eee4` (светлый)

## Css-переменные которые используются

```css
--color-accent: #d4fb72;      /* Лайм */
--background-primary: #101515; /* Темный */
--text-normal: #f2eee4;        /* Светлый текст */
--background-secondary: #17201f;
--color-orange: #ff9f5b;
```

## Особенности Minimal

- Боковая панель исчезает автоматически на узких экранах
- Таблицы автоматически становятся карточками при classе `cards`
- `cards-cols-3` = 3 колонки
- `cards-cols-2` = 2 колонки
- `hide-properties` = скрывает frontmatter

