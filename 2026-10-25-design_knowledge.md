# Предложенные дизайн-принципы — 2026-10-25

> Извлечены из дайджеста за 25 октября 2026. Ожидают одобрения дизайнера.

---

## 1. Компоненты & Паттерны

- **Принцип:** Именованные компоненты в DESIGN.md (например, «Primary Button», «Card — Default») дают AI-агенту значительно более точный результат, чем описание «сделай кнопку».
- **Почему:** Claude Design и Claude Code сопоставляют имя с полным набором свойств (размер, отступы, цвет, состояния), а при описании «от руки» угадывает параметры из общего обучения.
- **Источник:** [Set up your design system in Claude Design](https://support.claude.com/en/articles/14604397-set-up-your-design-system-in-claude-design) + [How I Use Claude Code Agent with VS Code as a Design System Designer](https://www.designsystemscollective.com/how-i-use-claude-code-agent-with-vs-code-as-a-design-system-designer-541e105c0c97)
- **Дата:** 2026-10-25

---

## 2. Figma-техники

- **Принцип:** В DESIGN.md хранить не только значения токенов, но и обоснование решений (почему именно этот spacing, почему такая иерархия цветов) — это позволяет AI-агенту корректно обрабатывать крайние случаи, не предусмотренные токенами напрямую.
- **Почему:** Обычный файл токенов говорит «что», но не «почему». Когда AI встречает ситуацию вне описанных правил, обоснование помогает ему принять решение в духе дизайн-системы, а не подставить дефолт.
- **Источник:** [Awesome Claude Design: 68 ready-to-use design systems in DESIGN.md format](https://github.com/VoltAgent/awesome-claude-design)
- **Дата:** 2026-10-25

---

## 3. Анти-паттерны

- **Принцип:** Не начинать работу с AI-инструментом без зафиксированных дизайн-токенов — размытый бриф без палитры, типографики и spacing-правил гарантирует «генеричный» результат, в котором виноват не AI, а входные данные.
- **Почему:** LLM генерирует «среднестатистический» дизайн по данным обучения, когда не получает конкретных ограничений. Фиксация токенов до первого промпта — единственный способ получить результат в стиле конкретного бренда.
- **Источник:** [Claude Code for Designers in 2026: Your AI Design Looking Generic Has Nothing to Do with the AI](https://tridipthrizu.medium.com/claude-code-for-designers-in-2026-your-ai-design-looking-generic-has-nothing-to-do-with-the-ai-2e977ed32ed7)
- **Дата:** 2026-10-25

---

*Ожидает ревью дизайнера*
