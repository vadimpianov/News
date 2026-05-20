# Предложенные дизайн-принципы — 2026-05-20

> Ожидают одобрения дизайнера. НЕ записаны в design_knowledge.md.

---

## 1. Анти-паттерны / AI-генерация

- **Принцип:** Для борьбы с «AI-эстетикой» задавайте явные CSS-значения (`border-radius: 0`, `font-family: 'Syne'`), а не абстрактные описания («make it modern»).
- **Почему:** AI-модели при расплывчатых инструкциях сходятся к одному и тому же generic стилю (gradient buttons, rounded cards, Inter/DM Sans). Жёсткие ограничения вынуждают модель генерировать уникальный визуал.
- **Источник:** [Claude Design: How to Build Branded Interfaces Without Generic AI Aesthetics](https://www.mindstudio.ai/blog/claude-design-avoid-generic-ai-aesthetics) — MindStudio
- **Дата:** 2026-05-20

---

## 2. Компоненты & Паттерны

- **Принцип:** Дизайн-система, загруженная в AI-инструмент при первом запуске, является главным рычагом качества — каждый последующий проект наследует токены, компоненты и правила.
- **Почему:** Без дизайн-системы AI генерирует visually coherent, но бренд-чужеродный результат. С ней — каждый прототип консистентен с продуктом команды, что сокращает ручную доводку на ~60%.
- **Источник:** [Upgrading my Design System with Claude Design](https://medium.com/ai-hero/upgrading-my-design-system-with-claude-design-0051f2204cfa) — Rahul Parundekar, AI Hero, май 2026
- **Дата:** 2026-05-20

---

## 3. Figma-техники

- **Принцип:** Консистентное именование слоёв, переменных и компонентов в Figma напрямую определяет качество работы AI-агента — «ваша неряшливость = ошибки Claude».
- **Почему:** AI-агенты (Claude Code + Figma MCP) парсят структуру файла буквально: broken references, дублированные стили и хаотичные имена приводят к ошибкам в генерации и неправильному маппингу компонентов.
- **Источник:** [How to make Claude Code follow your design system in Figma](https://uxdesign.cc/how-to-make-claude-code-follow-your-design-system-in-figma-559618cffaa9) — Sen Lin, UX Collective, май 2026
- **Дата:** 2026-05-20

---

*Принципы извлечены автоматически · ожидают ревью*
