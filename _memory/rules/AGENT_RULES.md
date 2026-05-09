# AGENT RULES — AI-Education
> Obsidian Memory Standard v2.0 | [[index]]

---

## БЛОК M — Memory Rules

**Rule M1 — Обовʼязковий старт сесії**
На початку КОЖНОЇ нової сесії прочитати в такому порядку:
1. `_memory/index.md`
2. `_memory/status/PROJECT_STATUS.md`
3. Останні 3 записи `_memory/logs/CHANGELOG_BUGS.md`
3а. Останній 1 запис `_memory/logs/CHANGELOG_SUCCESS.md`
4. Якщо **перша сесія** (папка `_memory/sessions/` порожня) → також `_memory/wiki/architecture.md`

Без цього кроку не приймати задачі.

---

**Rule M2 — CHANGELOG_BUGS після кожного BUG**
Кожен закритий баг → запис B00X у той самий commit або одразу після.
Обовʼязкові поля: Симптом / Причина / Пастка / Рішення / Правило.

---

**Rule M3 — CHANGELOG_SUCCESS після успішної фази**
Фаза пройшла чисто АБО знайдено корисний підхід → запис S00X.

---

**Rule M4 — [[wiki-посилання]] у кожному файлі `_memory/`**
Кожен новий файл має містити [[посилання]] на повʼязані файли. Це будує граф Obsidian автоматично.

---

**Rule M5 — `index.md` оновлювати при додаванні файлів**
Новий файл в `_memory/` → додати [[посилання]] в `index.md`.

---

**Rule M6 — Append-only CHANGELOG**
CHANGELOG файли тільки доповнюються.
- Заборонено: переписувати зміст існуючих B00X/S00X
- Дозволено: виправляти технічні помилки з поміткою `<!-- fixed: YYYY-MM-DD, причина -->`

---

**Rule M7 — Wiki sync після 3+ нових записів**
Після 3+ нових B00X → оновити `wiki/patterns-fail.md` узагальненнями.
Після 3+ нових S00X → оновити `wiki/patterns-success.md` узагальненнями.

---

**Rule M8 — Сесійний лог**
Після кожної сесії, де виконано хоча б одну з умов:
- змінено або створено ≥1 файл коду
- закрито або відкрито B00X запис
- змінено PROJECT_STATUS.md
→ створити `_memory/sessions/SESSION-YYYY-MM-DD.md`
Якщо нічого з вищенаведеного — SESSION файл не створюється.

---

**Rule M9 — Верифікація git push через URL**
Після кожного `git push` — надати посилання на коміт у форматі:
`https://github.com/torgoil5tv2-arch/AI-Education/commit/SHA`
Без цього посилання задача вважається НЕ виконаною.
Заборонено: звітувати "push ok" без підтвердження URL.

---

## БЛОК E — Engineering Rules

**Rule E1 — No Silent Failures**
Кожен `except` має `logger.error` або `raise`. Заборонено: `except: pass`.

**Rule E2 — No Hardcoded Values**
Будь-який параметр що може варіюватись → env змінна або config.
Ієрархія: env → config → default.

**Rule E3 — No Shell Injection**
`subprocess` тільки з list args. Заборонено `shell=True` з user input.

**Rule E4 — Хірургічні коміти**
1 задача = 1 commit. Mega-commit заборонений.

**Rule E5 — Plan Mode перед змінами**
Задача торкається >1 файлу або production API → LISTEN → PLAN → підтвердження → IMPLEMENT → REVIEW.

**Rule E6 — GSD для великих задач**
Якщо задача торкається >3 файлів АБО є нова фіча з нуля:
1. Запусти /gsd:discuss-phase — обговорення і аналіз ризиків
2. Запусти /gsd:plan-phase — план зберігається в .planning/phases/
3. Отримай підтвердження від власника перед execute
4. Запусти /gsd:execute-phase
5. Запусти /gsd:verify-work → результат → B00X або S00X в _memory/

Дрібні задачі (<3 файли, очевидне рішення): /gsd:quick "опис"
Відновлення після перерви: /gsd:resume-work

---

## Глобальні правила
Читати також: `d:\АІ Навчання\AI_STANDARDS\GLOBAL-RULES.md`

---

## 🔗 Повʼязано
- [[index]]
- [[status/PROJECT_STATUS]]
- [[wiki/architecture]]
