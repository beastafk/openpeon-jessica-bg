# Jessica BG

A bright, playful voice cheering you on in Bulgarian — an [OpenPeon](https://openpeon.com)
sound pack for [peon-ping](https://github.com/PeonPing/peon-ping).

42 spoken lines across all seven CESP categories, six per category so you
never hear the same line twice in a row and the pool takes a long time to
feel familiar.

## Install

```bash
peon packs install jessica-bg     # once listed in the registry
peon packs use jessica-bg
```

Or from a local clone:

```bash
git clone https://github.com/beastafk/openpeon-jessica-bg
peon packs install-local ./openpeon-jessica-bg
peon packs use jessica-bg
```

## Lines

| Category | Lines |
|---|---|
| `session.start` | Здравей! Готова съм! · Здрасти! Да започваме! · Тук съм! Да действаме. · На линия съм! · Хайде, да работим! · Включвам се. Казвай. |
| `task.acknowledge` | Разбрано! Започвам веднага. · Ясно! Заемам се. · Окей, действам! · Приех. Тръгвам. · Веднага! · Добре, гледам го. |
| `task.complete` | Готово! Успяхме! · Готово! Излезе чудесно. · Ето, свърших! · Финиш! Всичко е наред. · Изпълнено! · Приключих с това. |
| `task.error` | Опа! Нещо не се получи. · Ох! Появи се грешка. · Опа, счупи се нещо. · Ами... не стана. · Имаме проблем. · Тук нещо не е наред. |
| `input.required` | Чакам те! Кажи ми какво избираш. · Нужен си ми за момент! · Ти решаваш! Кажи. · Кажи ми как да продължа. · Твой ред е! · Спирам, докато не решиш. |
| `resource.limit` | Стигнах лимита! Не мога повече. · Свърших лимита! · Дотук бях, лимитът свърши. · Изчерпах се! · Горивото свърши! · Достигнах края. |
| `user.spam` | Спокойно, работя по въпроса! · Работя, работя! · Търпение, почти съм готова! · Чух те първия път! · Още малко, моля! · Не бързай толкова! |

`task.acknowledge` fires on every prompt you submit. peon-ping ships it
disabled by default; enable it in `config.json` if you want it.

## Audio

44.1 kHz mono MP3 at 96 kbps, silence-trimmed and loudness-matched per file
to about -14.6 LUFS with true peaks held at or below -1.3 dBTP. Clips run
0.9-1.8s. Graded GOLD by the registry's audio quality checker.

## Regenerating

`prompts.json` ships with the pack, so you can re-render any line with your own
ElevenLabs key:

```bash
peon eval jessica-bg
```

The voice is the stock ElevenLabs `Jessica` (`cgSgspJ2msm6clMCkdW9`), usable on
the free tier. Library voices are not.

## License

[CC BY-NC-4.0](LICENSE). Audio generated with ElevenLabs and additionally
subject to their terms.
