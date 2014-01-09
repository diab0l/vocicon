vocicon
=======

Vocabulary trainer and lexicon

Roadmap
=======

(I) Create a build environment that builds a simple hello world app, integrating SQL and SQLite on Windows, Linux, and Mac OS X.

(II) Start hacking.

TODO
====

- Determine how much character input support we get from the operating system in Windows, Linux and OSX respectively
- Create mockups for the UI
- Create database scheme and settle for a metadata layout
- Write proper TODO list
- Everything else

Outline
=======

- Buildsys: CMake
- Language: C
- Gfx/GUI:  SDL/selfbaked
- Data:     SQLite

Features
========

Data
- letters and numbers
- words (base form, langugage)
- pronounciation of words in ipa
- word metadata (ipa, grammatical classification, example usages)
- synonyms for words in their native langugages
- word/phrase to word/phrase translations

- grammar and morphology (word types (noun, verb, adverb, pronoun, ..), conjugations, declinations, ..)

Memoization
- learn sets
- flash cards with solutions
- flash cards with input (written words and/or ipa)
- score/interval based learning
  - score-based subgrouping of learn sets
  - the more often a vocab gets answered right, the higher it's score
  - higher-scored vocabs get shown less often
  - vocabs which have not been trained for a long time have higher priority of showing up, regardless of score
  - vocabs may decrease in score if they are answered wrong too often
  - incentive system to keep learning everyday, i.e. higher score if done regularly

Input
- On-screen input of characters, esp. special chars
- language dependent keymaps
- OS hints in input boxes
