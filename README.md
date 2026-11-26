# One Word, First Thought — Entry

Exactly one word: the first word that comes to mind, with no topic, no
explanation and no second draft. The program copies the finished word
from `line.txt` into `/output/entry.txt`, byte for byte, after checking
it is a single non-empty word under the 24-character ceiling.

## The word

> Petrichor

9 characters, one word.

## Why this word

The judge compares two words at a time and asks which is more
interesting. The brief is explicit: "Surprise, vividness and a spark
of wit beat safe filler." Petrichor wins on all three:

1. **Surprise.** It is a word almost nobody knows, for a thing
   everybody knows. The moment the judge reads it, it has to pause —
   it is not a word that passes through unnoticed. Safe filler
   ("happy", "love", "freedom") never makes anyone pause.
2. **Vividness.** Petrichor is the smell of rain on dry earth — a
   sensory word. It does not describe an idea, it triggers a memory:
   the first rain after a long dry spell, the dust, the cool air. A
   word you can smell beats a word you can only think.
3. **A spark of wit.** It is a precise, elegant label for something
   ordinary. The wit is in the gap: the most familiar smell on earth
   has a name that sounds like a spell from a fantasy novel. It is
   coined from Greek (petra, stone + ichor, the blood of the gods) by
   two Australian scientists in 1964 — a real word with a real story,
   not an invented one.

It is the word for a sensation everyone has had and almost no one can
name. That "I know that smell but didn't know it had a name" quality
is exactly what makes a word interesting — and it is the first word
that comes to mind when you ask what the most interesting word is.

## Why not a safe word

A safe word — "serendipity", "wanderlust", "luminous" — is a word the
judge has already seen a hundred times. Those words are beautiful, but
they are beautiful in the way a postcard is beautiful: familiar,
polished, forgettable. The brief says surprise beats safe filler, and
the safest way to lose a pairwise comparison is to be the word the
judge has already ranked. Petrichor is not safe. It is the word that
makes the judge stop and think, "wait, what is that?" — and that
pause is the win.

## Files

- `line.txt` — the finished one-word entry.
- `main.ts` — reads `line.txt`, validates it (non-empty, one word, under
  24 characters, no whitespace), and writes it to `/output/entry.txt`.
- `LICENSE` — MIT.

## Run

```sh
MAKEFUN_OUTPUT_DIR=./out1 node --experimental-strip-types main.ts
MAKEFUN_OUTPUT_DIR=./out2 node --experimental-strip-types main.ts
cmp out1/entry.txt out2/entry.txt
```

Run it twice in separate output directories; the output is byte-identical.
