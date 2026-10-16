# Предложенные дизайн-принципы — 2026-10-16

> Ожидают одобрения дизайнера перед добавлением в design_knowledge.md

---

## 1. Компоненты & Паттерны

- **Принцип:** При работе с AI-генерацией дизайна используй два раздельных канала обратной связи: чат для структурных изменений (layout, секции, direction), инлайн-комментарии для точечных правок (padding, spacing, component swaps) — смешивание замедляет итерацию.
- **Почему:** Источники (Design Systems Collective, Anthropic docs) описывают, что Claude Design оптимизирован под эту модель: чат перестраивает layout целиком, а инлайн-комментарий редактирует конкретный элемент без пересборки остальной страницы.
- **Источник:** [From Prompt to Production — Design Systems Collective](https://www.designsystemscollective.com/from-prompt-to-production-a-designers-step-by-step-workflow-with-claude-design-claude-code-a7705daad026)
- **Дата:** 2026-10-16

---

## 2. Figma-техники

- **Принцип:** При передаче дизайна из AI-инструмента в Figma используй промежуточный артефакт (handoff bundle с HTML + токены + компонентная структура), а не скриншот или ручное воссоздание — это сохраняет семантику слоёв и переменные.
- **Почему:** Прямой экспорт в Figma из Claude Design отсутствует, но bundle → html.to.design плагин → Figma сохраняет редактируемые слои, в отличие от flatten-копирования. Дизайнер Liam Goldfinch подтверждает: работа внутри определённой дизайн-системы при генерации критически влияет на качество handoff.
- **Источник:** [Claude Design to Figma: The html.to.design MCP Workflow — Sergei Chyrkov](https://sergeichyrkov.com/blog/claude-design-to-figma-with-html.to.design)
- **Дата:** 2026-10-16

---

## 3. Spacing & Layout

- **Принцип:** Для AI-генерации UI загружай токены spacing'а (не только цвета и шрифты) в дизайн-систему до начала работы — без них AI будет использовать произвольные значения отступов, и результат потребует полной переработки layout.
- **Почему:** Несколько источников (UISDC, IgnytLabs, Cal.com кейс) отмечают: цвета и типографика подхватываются автоматически из бренда, но spacing-токены часто игнорируются, если не заданы явно — это главная причина «generic» результата.
- **Источник:** [The Claude Design Workflow That Actually Works — Prajwal Tomar](https://x.com/PrajwalTomar_/article/2056347864822083809)
- **Дата:** 2026-10-16
