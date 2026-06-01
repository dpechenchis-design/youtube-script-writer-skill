# YouTube Script Writer — Dan Martell Framework

Claude Code skill для написання YouTube скриптів за структурою Dan Martell.

## Що це?

Skill автоматично генерує:
- **3-5 варіантів Title** (емоційні заголовки)
- **2-3 Thumbnail концепції**
- **Повний скрипт з таймкодами** (~8-18 хвилин)

## Структура скрипту

### PRE-PRODUCTION: 3T
| Елемент | Опис |
|---------|------|
| **Topic** | Валідація теми (TAM, search intent) |
| **Title** | Емоційні заголовки — страхи/блоки/мрії |
| **Thumbnail** | Крупний план + 3-5 слів тексту |

### HOOK: 3P Formula (перші 30 сек)
| Елемент | Опис |
|---------|------|
| **Proof** | Чому тебе слухати (credentials) |
| **Promise** | Що отримає глядач |
| **Plan** | 3 пункти відео |

### MAIN CONTENT: PEIL Cycles
Кожен пункт плану розкривається за структурою:
- **P**oint — називаємо ідею
- **E**xplain — пояснюємо чому важливо
- **I**llustrate — приклад або історія
- **L**esson — чітка інструкція

### ASYMMETRIC PACING
Прогресивне збільшення довжини секцій:
- Point 1: найкоротший (~1-2 хв)
- Point 2: середній (~2-3 хв)
- Point 3: найдовший (~3-4+ хв)

## Встановлення

### Варіант 1: Скопіювати в папку skills
```bash
mkdir -p ~/.claude/skills/youtube-script-writer
cp SKILL.md ~/.claude/skills/youtube-script-writer/
```

### Варіант 2: Використати як project skill
```bash
mkdir -p .claude/skills/youtube-script-writer
cp SKILL.md .claude/skills/youtube-script-writer/
```

## Використання

Просто скажи Claude Code:
```
напиши скрипт для ютуб про [твоя тема]
```

Або надай більше деталей:
```
Тема: [про що відео]
Ніша: [coaching / SaaS / marketing / etc.]
Proof: [твої credentials]
Цільова дія: [subscribe / book a call / download]
Тривалість: [short ~8 min / medium ~12 min / long ~18 min]
```

## Приклад Output

```
═══════════════════════════════════════════════════════════
YOUTUBE SCRIPT: Чому ти працюєш 12 годин і досі не багатий
Estimated length: ~12 minutes | Target: підприємці
═══════════════════════════════════════════════════════════

TITLES (pick one):
1. Чому ти працюєш 12 годин і досі не багатий
2. Я скоротив робочий день до 5 годин — ось що сталося
...

THUMBNAIL CONCEPTS:
• Здивоване обличчя + "12→5 ГОДИН" + перекреслений годинник
...

[0:00 - 0:30] HOOK
─────────────────────────────────────────────────────────
PROOF: ...
PROMISE: ...
PLAN: ...

[0:30 - 2:30] POINT 1: Пастка Зайнятості ⚡
─────────────────────────────────────────────────────────
**POINT** ...
**EXPLAIN** ...
**ILLUSTRATE** ...
**LESSON** ...
```

## Credits

Структура базується на YouTube framework від [Dan Martell](https://www.danmartell.com/).

## License

MIT
