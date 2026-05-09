# AI-Education — Memory Vault README

## Що це?

Це папка памʼяті проекту **AI-Education** — системи навчання Максима за стандартом **Obsidian Memory Standard v2.0**.

Усі файли тут зберігаються в Git і є **source of truth** для AI-агентів між сесіями.

---

## 🚀 Quickstart для Obsidian

```
Obsidian → Open another vault → Open folder as vault
→ Вибрати: d:\АІ Навчання\_memory\
```

### Базові налаштування Obsidian

| Розділ | Параметр | Значення |
|---|---|---|
| Editor | Default editing mode | Source mode |
| Editor | Strict line breaks | OFF |
| Files & Links | Default location for new notes | Same folder as current file |
| Files & Links | Use [[Wikilinks]] | ON |
| Files & Links | Automatically update internal links | ON |

### Graph view (Ctrl+G → ⚙️)
- `path:logs/` → червоний
- `path:wiki/` → синій
- `path:rules/` → жовтий
- `path:status/` → зелений

---

## 📁 Структура

```
_memory/
├── index.md                    ← точка входу (читати першим)
├── README.md                   ← цей файл
├── status/PROJECT_STATUS.md    ← активні задачі та фази
├── rules/AGENT_RULES.md        ← правила для агентів
├── logs/CHANGELOG_BUGS.md      ← B00X записи
├── logs/CHANGELOG_SUCCESS.md   ← S00X записи
├── wiki/architecture.md        ← архітектура проекту
├── wiki/patterns-fail.md       ← антипатерни
├── wiki/patterns-success.md    ← успішні патерни
├── wiki/memory-standard-changelog.md
├── sessions/                   ← логи сесій агентів
├── audits/                     ← аудити коду
├── decisions/                  ← архітектурні рішення (ADR)
└── templates/                  ← шаблони нових файлів
```

---

## 🔗 Посилання
- [[index]] — граф памʼяті
- Стандарт: `d:\АІ Навчання\AI_STANDARDS\OBSIDIAN-MEMORY-STANDARD-v1.1.md`
