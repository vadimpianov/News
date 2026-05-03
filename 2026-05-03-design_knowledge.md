# Предложенные дизайн-принципы — 3 мая 2026

> Ожидают одобрения дизайнера. НЕ добавлены в design_knowledge.md.

---

## 1. Компоненты & Паттерны

- **Принцип:** Дизайн-система должна быть описана в машинно-читаемом формате (CLAUDE.md / skill-файлы) с explicit constraints — это единственный способ получить non-generic output от AI-генерации.
- **Почему:** AI по умолчанию генерирует «safe average» — чистый, rounded, безликий дизайн. Уникальность результата прямо пропорциональна детализации правил, переданных AI (brand voice, spacing conventions, color constraints).
- **Источник:** https://tridipthrizu.medium.com/claude-code-for-designers-in-2026-your-ai-design-looking-generic-has-nothing-to-do-with-the-ai-2e977ed32ed7
- **Дата:** 3 мая 2026

---

## 2. Figma-техники

- **Принцип:** При работе с AI-генерацией используй «sandwich»-паттерн: задай design intent → получи 5-10 вариантов от AI → выбери и доведи лучший вручную в Figma, используя governance и collaboration.
- **Почему:** AI ускоряет exploration в 10x, но не умеет принимать решения о бренде, контексте пользователя и бизнес-ограничениях. Последние 10-20% — это то, что отличает профессиональный дизайн от «правильного среднего».
- **Источник:** https://medium.com/design-bootcamp/what-claude-design-actually-changes-for-designers-0c5b04fae343
- **Дата:** 3 мая 2026

---

## 3. Spacing & Layout

- **Принцип:** Дизайнер будущего проектирует не экраны, а «Design DNA» — систему токенов, spacing rules и layout constraints, которые AI использует как grammar для генерации любых экранов.
- **Почему:** Один набор правил (8px grid, breathing ratio, component spacing scale) масштабируется на бесконечное количество экранов через AI, тогда как ручной подход масштабируется линейно с количеством дизайнеров.
- **Источник:** https://medium.com/@uxraspberry/ux-design-2026-from-producing-to-deciding-from-craft-to-operation-e9c7ea6b1803
- **Дата:** 3 мая 2026
