# Предложенные дизайн-принципы — 2026-05-15

> Ожидают одобрения дизайнера. НЕ записывать в design_knowledge.md без ревью.

---

## 1. Компоненты & Паттерны

- **Принцип:** При работе с AI-генерацией в Figma создавайте отдельные Claude Code Skills для каждого слоя дизайн-системы (токены, компоненты, layout, naming conventions) — иначе AI будет использовать raw-значения вместо токенов.
- **Почему:** Claude Code умеет вызывать Figma API, но без явных правил проекта пишет #5C6AC4 вместо color/brand/primary и создаёт дубликаты вместо переиспользования компонентов из библиотеки. Skills — единственный способ обеспечить compliance на каждом слое.
- **Источник:** [How to make Claude Code follow your design system in Figma — Sen Lin, UX Collective](https://uxdesign.cc/how-to-make-claude-code-follow-your-design-system-in-figma-559618cffaa9)
- **Дата:** 2026-05-15

---

## 2. Spacing & Layout

- **Принцип:** Используйте 8-point grid как фундамент для всех spacing-значений в дизайн-токенах (8, 16, 24, 32...) — off-grid значения (7px, 13px) должны быть явно запрещены в системе.
- **Почему:** AI-инструменты (Claude Design, Claude Code) склонны генерировать произвольные значения spacing. Строгая сетка в дизайн-токенах обеспечивает визуальную консистентность даже при AI-генерации, и аудит-скиллы могут автоматически ловить off-grid отклонения.
- **Источник:** [Design Audit Claude Code Skill | Accessibility & UI Review](https://mcpmarket.com/tools/skills/design-audit-accessibility-review) + [Claude Design accessibility audit design tokens](https://github.com/Ashutos1997/claude-design-auditor-skill)
- **Дата:** 2026-05-15

---

## 3. Figma-техники

- **Принцип:** Используйте замкнутый цикл Claude Design → Claude Code → Figma Code to Canvas для итераций: прототип в Claude Design, реализация в Claude Code, импорт обратно в Figma для ручной доработки — это быстрее, чем вручную перестраивать прототип в Figma с нуля.
- **Почему:** Code to Canvas (Figma, февраль 2026) конвертирует production-код в полностью редактируемые Figma-фреймы со слоями, сохраняя структуру. Это устраняет главный разрыв — потерю контекста при передаче между инструментами. Гибридный воркфлоу позволяет использовать скорость AI на этапе идеации и точность Figma на этапе продакшна.
- **Источник:** [Claude Design, Figma MCP, Claude Code. The Full Loop — Medium/Bootcamp](https://medium.com/design-bootcamp/figma-stock-dropped-7-the-day-claude-design-launched-d94dcc06320c)
- **Дата:** 2026-05-15
