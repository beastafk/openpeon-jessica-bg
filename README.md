# Jessica BG

A bright, playful voice cheering you on in Bulgarian — an [OpenPeon](https://openpeon.com)
sound pack for [peon-ping](https://github.com/PeonPing/peon-ping).

21 spoken lines across all seven CESP categories, three per category so you
never hear the same line twice in a row.

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
| `session.start` | Здравей! Готова съм! · Здрасти! Да започваме! · Тук съм! Да действаме. |
| `task.acknowledge` | Разбрано! Започвам веднага. · Ясно! Заемам се. · Окей, действам! |
| `task.complete` | Готово! Успяхме! · Готово! Излезе чудесно. · Ето, свърших! |
| `task.error` | Опа! Нещо не се получи. · Ох! Появи се грешка. · Опа, счупи се нещо. |
| `input.required` | Чакам те! Кажи ми какво избираш. · Нужен си ми за момент! · Ти решаваш! Кажи. |
| `resource.limit` | Стигнах лимита! Не мога повече. · Свърших лимита! · Дотук бях, лимитът свърши. |
| `user.spam` | Спокойно, работя по въпроса! · Работя, работя! · Търпение, почти съм готова! |

`task.acknowledge` fires on every prompt you submit. peon-ping ships it
disabled by default; enable it in `config.json` if you want it.

## Audio

44.1 kHz mono 16-bit WAV, normalised to roughly -15 dB mean with peaks at
-1 dB, silence-trimmed. Clips run 0.9–1.8s.

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
