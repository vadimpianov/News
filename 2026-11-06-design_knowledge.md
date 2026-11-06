# Предложенные дизайн-принципы — 2026-11-06

> Ожидают одобрения дизайнера. НЕ записаны в design_knowledge.md.

---

## 1. Компоненты & Паттерны

**Принцип:** При работе с AI-генерацией UI всегда загружай дизайн-систему до первого промпта — без неё результат будет визуально «красивым, но безликим» и не пригодным для продакшена.

**Почему:** Все практические обзоры Claude Design (октябрь 2026) сходятся в том, что качество генерации радикально отличается «с дизайн-системой» vs «без»: с ней Claude использует реальные токены, палитру, типографику и компоненты проекта, без неё — изобретает generic стиль, который потом всё равно придётся переделывать.

**Источник:** [Karo Zieminski — Claude Design Review: 48-Hour Builder's Test](https://karozieminski.substack.com/p/claude-design-review-prompts-figma), [Anima Blog — Claude Design Review](https://animaapp.com/blog/ai-design-en/claude-design-review-features-pros-cons-and-best-alternatives/)

**Дата:** 2026-11-06

---

## 2. Figma-техники

**Принцип:** Мелкие визуальные правки (отступы, выравнивание, цвет отдельного элемента) делай вручную в Figma, а не через перепромпчивание AI — это экономит токены и не ломает соседние элементы макета.

**Почему:** Практический воркфлоу от Design Systems Collective показывает, что AI-инструмент при повторном промпте может непредсказуемо изменить другие части макета. Ручная финализация в Figma точнее и быстрее для микро-правок, а Claude Code при этом распознаёт ручные изменения и итерирует поверх них.

**Источник:** [Design Systems Collective — Claude + Figma in the Real World](https://www.designsystemscollective.com/claude-figma-in-the-real-world-a-simple-step-by-step-workflow-for-teams-90331e988e0c)

**Дата:** 2026-11-06

---

## 3. Анти-паттерны

**Принцип:** Не пытайся дизайнить и кодить в одном AI-разговоре — разделяй визуальную разведку (Design) и реализацию (Code) в отдельные сессии с чётким хэндоффом между ними.

**Почему:** Множественные обзоры (Geeky Gadgets, Staragile, DEV.to) фиксируют, что смешивание design- и code-задач в одном контексте приводит к путанице: AI теряет фокус, генерирует «ни рыба ни мясо». Handoff через Export → Claude Code обеспечивает чистую передачу дизайн-решений в код без потери контекста.

**Источник:** [Geeky Gadgets — Avoid Generic AI Design with Claude](https://www.geeky-gadgets.com/avoid-generic-ai-design-claude/), [Design Systems Collective — From Prompt to Production](https://www.designsystemscollective.com/from-prompt-to-production-a-designers-step-by-step-workflow-with-claude-design-claude-code-a7705daad026)

**Дата:** 2026-11-06
