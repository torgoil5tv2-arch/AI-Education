# Architecture — AI-Education
> Огляд архітектури проекту | [[index]]

---

## Проект

**Назва**: AI-Education
**Мета**: Система навчання Максима — структуровані навчальні матеріали, завдання та проекти за допомогою AI-агентів
**GitHub**: https://github.com/torgoil5tv2-arch/AI-Education
**Власник**: Батько Максима (torgoil5tv2-arch)

---

## Стек

> ⚠️ Проект на початковому етапі. Стек буде уточнено після створення перших навчальних модулів.

| Компонент | Технологія | Примітка |
|---|---|---|
| Навчальні матеріали | Markdown / HTML | Основний формат |
| AI-агенти | Claude (Anthropic) | Antigravity / Claude Code |
| Система памʼяті | Obsidian Memory Standard v2.0 | `_memory/` структура |
| Версійний контроль | Git / GitHub | torgoil5tv2-arch/AI-Education |
| ОС | Windows | PowerShell |

---

## Структура папок

```
d:\АІ Навчання\
├── AI_STANDARDS\          ← Obsidian Memory Standard (стандарти)
│   ├── OBSIDIAN-MEMORY-STANDARD-v1.1.md
│   ├── MASTER-SETUP-PROMPT.md
│   ├── AGENT-INIT-PROMPT.md
│   ├── CLAUDE.md.template
│   ├── ROADMAP.md
│   ├── init-memory.ps1
│   ├── sync-global-rules.ps1
│   └── files.zip
├── _memory\               ← Пам'ять проекту (цей vault)
│   ├── index.md
│   ├── status\
│   ├── rules\
│   ├── logs\
│   ├── wiki\
│   ├── sessions\
│   ├── audits\
│   ├── decisions\
│   └── templates\
└── CLAUDE.md              ← Автоматичні інструкції для Claude
```

---

## Ключові файли

| Файл | Призначення |
|---|---|
| `AI_STANDARDS/OBSIDIAN-MEMORY-STANDARD-v1.1.md` | Головний стандарт системи памʼяті |
| `AI_STANDARDS/MASTER-SETUP-PROMPT.md` | Промт для налаштування нових проектів |
| `AI_STANDARDS/init-memory.ps1` | PowerShell скрипт ініціалізації |
| `_memory/index.md` | Точка входу для агентів |
| `_memory/status/PROJECT_STATUS.md` | Поточний стан проекту |
| `CLAUDE.md` | Інструкції для Claude Code (автозавантаження) |

---

## Ключові обмеження

1. **Git не в PATH** — на поточній машині `git` не знайдено через PowerShell PATH. Потрібно вирішити або використовувати повний шлях до git.exe.
2. **GitHub репо** — https://github.com/torgoil5tv2-arch/AI-Education (може бути приватним або ще не створеним)
3. **Навчальна мета** — проект орієнтований на Максима, тому контент має бути адаптований до його рівня та інтересів

---

## Канонічні команди

```powershell
# Перехід до проекту
cd "d:\АІ Навчання"

# Оновлення глобальних правил (якщо є інші проекти)
d:\АІ Навчання\AI_STANDARDS\sync-global-rules.ps1
```

---

## 🔗 Повʼязано
- [[index]]
- [[status/PROJECT_STATUS]]
- [[rules/AGENT_RULES]]
