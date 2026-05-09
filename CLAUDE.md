# AI-Education — Claude Instructions

> Проект навчання Максима | Obsidian Memory Standard v2.0

---

## ОБОВʼЯЗКОВИЙ СТАРТ СЕСІЇ

Перед будь-якою роботою прочитати в такому порядку:

1. `_memory/index.md`
2. `_memory/status/PROJECT_STATUS.md`
3. Останні 3 записи `_memory/logs/CHANGELOG_BUGS.md`
4. Останній 1 запис `_memory/logs/CHANGELOG_SUCCESS.md`
5. Якщо перша сесія (sessions/ порожня) → також `_memory/wiki/architecture.md`

**Без цього кроку не приймати задачі.**

---

## ПРОЕКТ

**Назва**: AI-Education
**Мета**: Навчання Максима з використанням AI-агентів
**GitHub**: https://github.com/torgoil5tv2-arch/AI-Education
**Стек**: Markdown / HTML / Python (уточнюється)
**Репо**: `d:\АІ Навчання`
**Vault**: `d:\АІ Навчання\_memory\`

---

## СТАНДАРТ ПАМʼЯТІ

Цей проект використовує **Obsidian Memory Standard v2.0**.
Повний стандарт: `d:\АІ Навчання\AI_STANDARDS\OBSIDIAN-MEMORY-STANDARD-v1.1.md`
Правила: `_memory/rules/AGENT_RULES.md` (M1–M9, E1–E6)
Глобальні правила: `d:\АІ Навчання\AI_STANDARDS\GLOBAL-RULES.md`

---

## GSD КОМАНДИ

- Нова велика задача (>3 файли): `/gsd:discuss-phase` → `/gsd:plan-phase` → підтвердження → `/gsd:execute-phase` → `/gsd:verify-work`
- Дрібна задача: `/gsd:quick "опис"`
- Відновлення сесії: `/gsd:resume-work`

---

## КЛЮЧОВІ ПРАВИЛА

| Правило | Дія |
|---|---|
| M2 | Кожен закритий баг → B00X в `_memory/logs/CHANGELOG_BUGS.md` |
| M3 | Успішна фаза → S00X в `_memory/logs/CHANGELOG_SUCCESS.md` |
| M6 | CHANGELOG тільки доповнюється, ніколи не переписується |
| M8 | Сесія зі змінами → `_memory/sessions/SESSION-DATE.md` |
| M9 | Після git push → надати URL коміту |
| E1 | No silent failures (`except: pass` заборонено) |
| E4 | 1 задача = 1 commit |
| E5 | Задача >1 файлу → PLAN перед IMPLEMENT |
| E6 | Задача >3 файлів → GSD workflow |

---

## ШПАРГАЛКА

| Подія | Дія |
|---|---|
| Нова сесія | Читати index + STATUS + 3 BUGS + 1 SUCCESS |
| Баг закрито | B00X в CHANGELOG_BUGS |
| Фаза успішна | S00X в CHANGELOG_SUCCESS |
| Новий файл в `_memory/` | Додати [[посилання]] в index.md |
| 3+ нових B00X | Оновити wiki/patterns-fail.md |
| 3+ нових S00X | Оновити wiki/patterns-success.md |
| Сесія зі змінами | Створити sessions/SESSION-DATE.md |
| Важливе рішення | Створити decisions/ADR-00X.md |
