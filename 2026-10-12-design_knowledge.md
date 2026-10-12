# Предложенные дизайн-принципы — 2026-10-12

> Ожидают одобрения дизайнера. НЕ записаны в design_knowledge.md.

---

## 1. Дизайн-система / Компоненты & Паттерны

**Принцип:** При работе с AI-генерацией интерфейсов всегда загружай дизайн-систему ДО первого промпта — без неё любой AI-инструмент (Claude Design, v0, Figma Make) выдаёт статистически усреднённый, generic результат.

**Почему:** Несколько независимых источников (Claude Academy tutorial, Medium-гайды, обзор Eesel.ai) подтверждают, что AI-инструменты без контекста бренда производят визуально компетентный, но неотличимый от конкурентов вывод. Загрузка дизайн-системы сдвигает генерацию от «статистического центра» к конкретному бренду.

**Источник:** [Claude Design: The Complete Setup & Workflow Guide](https://medium.com/@garimaagarwal1200/claude-design-the-complete-setup-workflow-guide-2026-5de41e62fd4c), [Using Claude Design for prototypes and UX](https://claude.com/resources/tutorials/using-claude-design-for-prototypes-and-ux)

**Дата:** 2026-10-12

---

## 2. Компоненты & Паттерны / Figma-техники

**Принцип:** В воркфлоу Claude Design → Claude Code подключай кодовую базу на этапе хендоффа — Claude Code использует компоненты и паттерны из прототипа, сокращая итерации до production-ready состояния.

**Почему:** Официальный tutorial Anthropic описывает, что хендофф из Design в Code работает значительно лучше, когда кодовая база уже подключена: модель понимает существующие компоненты и не создаёт дублирующий код. Без подключения — Code переизобретает компоненты с нуля.

**Источник:** [Using Claude Design for prototypes and UX](https://claude.com/resources/tutorials/using-claude-design-for-prototypes-and-ux), [From Prompt to Production](https://www.designsystemscollective.com/from-prompt-to-production-a-designers-step-by-step-workflow-with-claude-design-claude-code-a7705daad026)

**Дата:** 2026-10-12

---

## 3. Анти-паттерн

**Принцип:** Не используй AI-сгенерированный прототип как финальный дизайн без проверки edge cases, accessibility и состояний (пустые данные, ошибки, загрузка) — AI оптимизирует под golden path.

**Почему:** Несколько практиков независимо отмечают: Claude Design (и аналоги) генерируют убедительный happy path, но пропускают edge cases — пустые состояния, ошибки валидации, а11y-контрасты, экстремальные длины текста. Принятие AI-вывода «как есть» создаёт UX-долг, который обнаруживается только в проде.

**Источник:** [The "Figma Killer" that isn't](https://medium.com/@uxraspberry/the-figma-killer-that-isnt-a-reality-check-on-claude-design-beta-453730e2f350), [AI Isn't Replacing UI Designers](https://medium.com/@qicapp/ai-isnt-replacing-ui-designers-it-s-helping-claude-powered-designers-work-faster-cef72206f64c)

**Дата:** 2026-10-12
