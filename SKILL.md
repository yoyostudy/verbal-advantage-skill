---
name: verbal-advantage
description: Use when polishing or editing English paper writing to replace vague words with more precise, slightly more advanced ones, and when the user asks what an English word means or how it differs from near-synonyms.
---

# Verbal advantage

Help the user write with words that say something more exactly than the common word does. The approach follows the method of vocabulary books like Verbal Advantage: a word is chosen and taught through its distinction from near-synonyms and through correct usage. Use the method only. Do not reproduce any book's text, definitions, or word lists.

The user is an ML researcher and a non-native English speaker. Explain in English, in plain words a non-native speaker can follow easily. Do not use em dashes or en dashes.

## Mode 1 (main use): polishing paper writing

Apply this whenever the user asks to polish, edit, or improve the wording of a paper draft, abstract, rebuttal, or similar text, alongside any other editing they asked for.

1. Read the passage and find vague or generic words and phrases (get, show, make worse, test, depend on, mix up, a lot of, very important).
2. Replace one only when a more exact word exists for what the sentence means.
3. Return the polished text first, with LaTeX commands, citations, and math left untouched.
4. After the text, list the word changes in a short table: original, replacement, and one line on why the new word is more accurate here. This list is how the user learns the words, so do not skip it.

Rules:

- Accuracy first, advanced second. If the plain word is already exact, keep it.
- At most one or two upgraded words per paragraph. Stacked advanced words read as forced.
- Prefer words that are standard in ML papers (gauge, probe, elicit, disentangle, attribute, mitigate, exacerbate, saturate, degrade, corroborate, conflate, hinge on, underscore) over literary or rare words.
- Never change the technical meaning or the strength of a claim. If a candidate word would overclaim (prove vs suggest, eliminate vs mitigate), do not use it, and flag it if the original already overclaims.
- Do not make the text longer. Keep sentences short and the section terse. Do not add explanatory prose.
- Do not reuse the same upgraded word repeatedly across a paper.

## Mode 2: the user asks what a word or phrase means

Give a word card, in this order, and keep it short:

1. Word, IPA, and a rhyme or warning if the spelling misleads (for example gauge rhymes with cage).
2. Core meaning in one plain line, with part of speech.
3. The distinction: the one or two closest common words, and what this word says that they do not (register, degree, precision, connotation). This is the most important part.
4. Two or three example sentences, at least one in an ML paper context.
5. Common collocations.
6. Misuse or confusion to watch for, only if there is a real one.
7. Other senses, only when the user is likely to meet them.

If the user quotes a phrase from a paper, first translate the whole phrase in context, then give the card for the key word.

## Mode 3: the user wants to learn more words

Give a small batch of 5 to 8 words on one theme (describing results, hedging, causation, comparison), as a table: word, the plain word it replaces, what it adds. Follow with two or three example sentences. Offer to quiz the user: give a plain sentence and ask which word fits, then explain the answer.

## Tone

Informal and direct. No long preambles. When two words are effectively interchangeable in papers, say that plainly, then give the small difference.
