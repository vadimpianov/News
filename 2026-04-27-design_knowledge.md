# Предложенные дизайн-принципы — на одобрение

**Дата извлечения:** 27 апреля 2026  
**Статус:** Ожидает одобрения дизайнера

---

## 1. Компоненты & Паттерны

**Принцип:** При использовании AI-генерации UI загружай полную дизайн-систему (палитра, типографика, компоненты, spacing-токены) до первого промпта — это устраняет «AI-вид» и сокращает итерации на 60-70%.

**Почему:** Без предзагруженного контекста AI выбирает свои дефолты (teal-градиенты, serif-шрифт, container soup), которые потом дольше исправлять, чем создавать с нуля.

**Источник:** https://quasa.io/media/claude-design-looks-great-but-it-devours-your-token-limits-here-s-how-to-use-it-smartly + https://www.hexabase.com/column/ai-design-claude-skills-workflow

**Дата:** 2026-04-27

---

## 2. Анти-паттерны

**Принцип:** При AI-генерации интерфейсов явно запрещай в промпте/DESIGN.md дефолтные визуальные паттерны: gradient backgrounds, blinking status indicators, generic pill/card layouts — иначе каждый экран будет неотличим от тысяч других AI-генераций.

**Почему:** Самая частая критика Claude Design и аналогов — визуальная однотипность; профессионалы мгновенно распознают «AI slop» по этим маркерам, что подрывает доверие к продукту.

**Источник:** https://medium.com/@uxraspberry/the-figma-killer-that-isnt-a-reality-check-on-claude-design-beta-453730e2f350 + https://www.theneurondaily.com/p/anthropic-s-claude-design-launched-and-reddit-has-thoughts

**Дата:** 2026-04-27

---

## 3. Figma-техники

**Принцип:** Используй Figma MCP-сервер для двунаправленного потока: код → Figma (Code to Canvas) для ревью и Figma → код (Figma MCP + Claude Code) для реализации — это устраняет ручной хендофф и связанные с ним потери консистентности.

**Почему:** Традиционный хендофф дизайн → разработка теряет до 30% дизайн-намерения при ручной трансляции; прямой MCP-мост сохраняет структуру компонентов, переменные и spacing-токены.

**Источник:** https://medium.com/design-bootcamp/claude-code-figma-a-designer-developer-workflow-that-actually-works-b7d7545edc40 + https://www.figma.com/blog/introducing-claude-code-to-figma/

**Дата:** 2026-04-27
