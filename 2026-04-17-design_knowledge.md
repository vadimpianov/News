# Предложенные дизайн-принципы — 17 апреля 2026
> Статус: **ожидают одобрения дизайнера**. Не добавлены в design_knowledge.md.

---

## Компоненты & Паттерны

**Принцип:** Начинай работу AI-агента в Figma с отдельного компонента, а не с целой страницы — это даёт точнее управляемый результат.

**Почему:** Claude (и любой AI-агент) теряет точность при большом контексте; изолированный компонент — это ограниченная, чёткая задача, которую модель решает качественно.

**Источник:** [Designers, Try This: Claude + Figma Workflow Hack — Medium](https://medium.com/@ahirlog/designers-try-this-claude-figma-workflow-hack-4a053f883609) + [Figma MCP workflow guides]

**Дата:** 17 апреля 2026

---

## Figma-техники

**Принцип:** Передавай Claude «философию дизайн-системы» (токены, компоненты, правила) в начале сессии — это устраняет «generic» вид AI-генерируемого UI.

**Почему:** AI не знает твою систему — без контекста он генерирует усреднённый Bootstrap-стиль; с контекстом выдаёт компоненты уровня senior-дизайнера.

**Источник:** [Claude code for Designers in 2026 — Medium](https://tridipthrizu.medium.com/claude-code-for-designers-in-2026-your-ai-design-looking-generic-has-nothing-to-do-with-the-ai-2e977ed32ed7)

**Дата:** 17 апреля 2026

---

## Анти-паттерны

**Принцип:** Не делегируй AI стратегические дизайн-решения — только рутинные операции (токены, аудиты, документация, генерация вариантов).

**Почему:** AI оптимизирует под «среднее» — уникальный продуктовый голос и системное мышление остаются человеческой задачей; делегирование стратегии ведёт к commodity-дизайну.

**Источник:** [Vibe Design in 2026 — Muzli Blog](https://muz.li/blog/vibe-design-in-2026-what-ai-generated-ui-means-for-your-work/) + [Using Claude Code SMARTLY — Medium](https://medium.com/@christina0w0/using-claude-code-smartly-as-a-product-ux-designer-7feb3343d355)

**Дата:** 17 апреля 2026
