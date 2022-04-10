# Notes on flashcard collections

A collection of flashcards has

- a list of cards
- a list of decks containing unique card ids

A collection is the primary method of distributing flashcards. They contain all the card material (front/back), as well as standard decks that make sense for these cards. For example, for learning Chinese, standard decks are "HSK" categories.

A deck is a secondary method of distributing flashcards. It is possible to extend a collection with additional decks for training particular subsets; e.g. the first words of HSK are called "HSK 1", but the entire vocabulary of the first chapter of the HSK 1 book may be another subset.

## Flashcard identifiers

Flashcard software will need to have identifiers of flashcards for several reasons. Both for recording statistics on individual flashcards, and for expressing subsets of flashcard collections without repeating the content itself. As a default, picking [UUID][uuid]s may seem like a good choice. They're 128 bits and are intended as universally unique.

But for larger flashcard collections, I wonder if we would actually prefer something much smaller that is actually not unique, but is a digest of its content. Perhaps, even, not requiring any specific format has no downside.

Maybe a hierarchical namespace of "collection/card" where "card" could itself be arbitrarily sub-namespaced? I'd like a collection of flashcards with different varieties, e.g.

- ones with the hanzi characters on the front, 
- ones with the hanzi + audio on the front,
- ones with 

[uuid]: https://en.wikipedia.org/wiki/Universally_unique_identifier