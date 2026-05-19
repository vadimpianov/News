# Предложенные дизайн-принципы — 2026-05-19

> Ожидают одобрения дизайнера. НЕ записаны в design_knowledge.md.

---

## 1. Анти-паттерны

**Принцип:** Запретите AI использовать «заезженные» шрифты (Inter, Roboto, Arial, Space Grotesk) через Taste Skill — это главный рычаг против generic AI-output.

**Почему:** AI-модели по умолчанию тяготеют к самым распространённым шрифтам из обучающих данных; явный запрет заставляет модель искать более выразительные и уникальные решения, что сразу отличает результат от «AI-слопа».

**Источник:** [I Tried 8 Claude Skills for UI/UX: Here's What Actually Stuck — Khoerul Umam](https://khumam.medium.com/i-tried-8-claude-skills-for-ui-ux-heres-what-actually-stuck-80da68a7d40f)

**Дата:** 2026-05-19

---

## 2. Дизайн-системы & Figma-техники

**Принцип:** Создайте enforcement layer из отдельных Skills (валидация токенов, проверка компонентов, контроль стилей, применение структуры) вместо одного промпта — Claude может генерировать pixel-perfect результат, не используя реальные токены из библиотеки.

**Почему:** Визуальная корректность ≠ системная корректность; без enforcement layer Claude «подделывает» стили вместо использования настоящих design tokens, что ломает консистентность при масштабировании.

**Источник:** [How to make Claude Code follow your design system in Figma — Sen Lin, UX Collective](https://uxdesign.cc/how-to-make-claude-code-follow-your-design-system-in-figma-559618cffaa9)

**Дата:** 2026-05-19

---

## 3. Spacing & Layout

**Принцип:** Фиксируйте design tokens (цвета, типографика, spacing на 8px base grid, border-radius) до генерации любых экранов — «system first, screens second».

**Почему:** Если токены не зафиксированы заранее, каждый сгенерированный экран использует свои значения, и дизайн-система превращается в набор несвязанных артефактов; подход «система-первая» гарантирует, что все экраны наследуют единый визуальный язык.

**Источник:** [How to Avoid AI Slop When Using Claude Design — MindStudio](https://www.mindstudio.ai/blog/claude-design-avoid-ai-slop-design-system) + [Upgrading my Design System with Claude Design — Rahul Parundekar](https://medium.com/ai-hero/upgrading-my-design-system-with-claude-design-0051f2204cfa)

**Дата:** 2026-05-19

---

*Принципы ожидают одобрения дизайнера. После утверждения — перенести в design_knowledge.md.*
