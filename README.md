# verbal-advantage

A Claude skill for precise English wording in research writing.

It does three things:

1. **Polish paper writing.** Replaces vague words with more exact ones, returns the polished text, then lists each change with a one-line reason.
2. **Explain a word.** Pronunciation, core meaning, how it differs from its nearest common synonyms, ML-paper examples, collocations.
3. **Teach a batch of words.** 5 to 8 words on one theme, with an optional quiz.

Explanations are in Chinese by default.

## What is Verbal Advantage?

[*Verbal Advantage: Ten Easy Steps to a Powerful Vocabulary*](https://www.penguinrandomhouse.com/books/46291/verbal-advantage-by-charles-elster/) is a vocabulary book by Charles Harrington Elster (Random House Reference, 2000), adapted from his audio course of the same name. It is organized as ten levels of increasing difficulty. What sets it apart from a word list is how each word is taught: pronunciation, exact meaning, word history, how it differs from its synonyms, and how it is commonly misused.

This skill borrows that teaching method and applies it to research writing: a word is worth using only if it says something more exactly than the common word. The skill contains no text, definitions, or word lists from the book.

## Install

Claude Code:

```bash
git clone https://github.com/yoyostudy/verbal-advantage-skill ~/.claude/skills/verbal-advantage
```

Then invoke it with `/verbal-advantage`, or just ask Claude to polish a paragraph.

Claude app: upload `SKILL.md` as a custom skill in your skill settings.

## Example

Input:

> NIAH is too easy now, so it cannot show the difference between models.

Output:

> NIAH has largely saturated, so it no longer gauges meaningful differences between models.

| Original | Replacement | Why |
|---|---|---|
| is too easy now | has largely saturated | saturate 专指 benchmark 被刷满、失去区分度 |
| show | gauge | gauge 是"衡量水平"，比 show 更贴合评测语境 |
