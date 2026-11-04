# Предложенные дизайн-принципы — 2026-11-04

> Ожидают одобрения дизайнера. НЕ записаны в design_knowledge.md.

---

## 1. Компоненты & Паттерны

**Принцип:** Разделяй skill.md (что делать) и DESIGN.md (почему так) — skill содержит триггеры и команды, DESIGN содержит обоснования дизайн-решений и значения токенов.

**Почему:** Это позволяет переиспользовать один skill для разных проектов, меняя только DESIGN.md, и обеспечивает консистентность AI-генерируемого UI без ручных правок.

**Источник:** [I Built a Claude Code Skill That Turns a Design System into Pixel-Perfect UI](https://medium.com/@gravitano/i-built-a-claude-code-skill-that-turns-a-design-system-into-pixel-perfect-ui-heres-how-6d00c90daccd)

**Дата:** 2026-11-04

---

## 2. Figma-техники

**Принцип:** При проектировании user flows в Claude Design сначала описывай информационную архитектуру и пользовательский путь текстом, и только потом переходи к визуальному проектированию.

**Почему:** Claude Design генерирует более связные и логичные интерфейсы, когда получает контекст полного пользовательского сценария, а не запрос на отдельный экран — это уменьшает количество итераций и правок.

**Источник:** [Claude Design for UX: How to Design Complete User Flows, Not Just UI Screens](https://uxplanet.org/claude-design-for-ux-how-to-design-complete-user-flows-not-just-ui-screens-094d6b8a7855)

**Дата:** 2026-11-04

---

## 3. Анти-паттерны

**Принцип:** «AI-эстетика» в интерфейсах — не проблема модели, а отсутствие дизайн-контекста; генерик-UI исчезает, когда Claude получает конкретные правила типографики, цветовой палитры и spacing проекта.

**Почему:** Без загруженной дизайн-системы Claude использует свои дефолтные решения (одинаковые для всех), что и создаёт узнаваемый «AI-стиль». Контекст проекта — единственное решение этой проблемы.

**Источник:** [Claude code for Designers in 2026: Your AI design looking generic has nothing to do with the AI](https://tridipthrizu.medium.com/claude-code-for-designers-in-2026-your-ai-design-looking-generic-has-nothing-to-do-with-the-ai-2e977ed32ed7)

**Дата:** 2026-11-04

---

*Файл создан автоматически. Принципы ожидают одобрения дизайнера перед записью в design_knowledge.md.*
