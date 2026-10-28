# Предложенные дизайн-принципы — 2026-10-28

> Извлечено из дайджеста за 28 октября 2026. Ожидает одобрения дизайнера.

---

## 1. Компоненты & Паттерны

**Принцип:** Дизайн-система должна быть настроена ДО первого промпта в AI-дизайн-инструменте — это определяет качество всех последующих генераций.

**Почему:** Множество практиков (Claude Design guides, RAR Design, UISDC) подтверждают: без загруженной дизайн-системы AI генерирует generic-результаты. Настройка ДС — одноразовая инвестиция, которая определяет потолок качества всех будущих артефактов.

**Источник:** [Claude Design: The Complete Setup & Workflow Guide (2026)](https://www.designsystemscollective.com/claude-design-the-complete-setup-workflow-guide-2026-5de41e62fd4c), [Claude Code for Designers in 2026 — Tridip Thrizu](https://tridipthrizu.medium.com/claude-code-for-designers-in-2026-your-ai-design-looking-generic-has-nothing-to-do-with-the-ai-2e977ed32ed7)

**Дата:** 2026-10-28

---

## 2. Figma-техники

**Принцип:** Используйте Tweaks-слайдеры и прямое редактирование canvas для микро-правок вместо текстовых промптов — это экономит 5-15 минут на каждой итерации генерации.

**Почему:** Каждый текстовый промпт запускает полный цикл генерации (5-15 минут). Tweaks позволяют менять шрифты, радиусы, отступы мгновенно и без потери контекста текущего дизайна. Это разница между «работать быстро» и «ждать AI».

**Источник:** [Claude Design: A Designer's Walkthrough and Honest Take](https://medium.com/design-bootcamp/claude-design-a-designers-walkthrough-and-honest-take-ec844d822cd5), [Honest Review on Claude Design — Kay Zhang](https://kay-zhang.com/blog/honest-review-on-claude-design/)

**Дата:** 2026-10-28

---

## 3. Компоненты & Паттерны

**Принцип:** Оформляйте повторяющиеся дизайн-процессы (аудит, синтез исследований, critique) как переиспользуемые Claude Skills с явными anti-patterns и clarifying questions.

**Почему:** Skills превращают неформализованное знание дизайнера в воспроизводимый процесс. Ключ — указать anti-patterns явно («не генерируй generic рекомендации», «не пропускай accessibility»), потому что модель стремится угодить и без явных ограничений даёт поверхностные результаты.

**Источник:** [How I Use Claude Skills in My Design Process — Tepphy Juliana](https://medium.com/@tepphy.juliana25/how-i-use-claude-skills-to-run-workflows-in-my-design-process-as-a-product-designer-6866a34110fe), [Claude Skills for Product Designers — Figma Resource Library](https://www.figma.com/resource-library/claude-skills-for-product-designers/)

**Дата:** 2026-10-28

---

*Принципы ожидают одобрения. Не записывать в design_knowledge.md без подтверждения дизайнера.*
