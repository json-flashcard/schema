# JSON Flashcard Schemas

This repository contains [JSON Schema][json-schema] definitions for JSON Flashcard.

## `draft/2022-04`

**This draft is a work in progress. It is subject to radical change.**

The [`draft/2022-04`](./draft/2022-04) schema aims for a basic coverage of flashcards, collections of flashcards and subsets of collections. The purpose of this draft is to consider distributing flashcards, and referring to flashcards from one or more distributions. In this draft, all content of the flashcards themselves have `"type": "string"`, so it does not address embedding multimedia like HTML or audio/video. This draft also does not yet cover recording spaced-repetition metadata. The intent is to get a good understanding of each layer of a well-functioning flashcard systems.

[json-schema]: http://json-schema.org/
