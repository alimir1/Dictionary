# Dictionary
A Swift library to perform word searches in a dictionary

**Author:** Ali Mir
**Date:** June 7, 2018

# Installation
Simply drag [`Dictionary.swift`](/Dictionary.swift) to your project.

# Usage
Create an instance of `Dictionary`.
`words(with prefix: String)` - returns all words with given prefix
`isValid(word: String)` - A Boolean that indicates if a given String is a valid word in the English dictionary.
`isValid(prefix: String)` - A Boolean that indicates if a given String is a valid prefix in English dictionary.

# Example
`SWIFT
let dict = Dictionary()
print(dict.words(with: "animal"))
print(dict.isValid(word: "animal"))
print(dict.isValid(prefix: "joe"))
`

## Notes
This library uses a [Trie](https://en.wikipedia.org/wiki/Trie) (aka Prefix Tree) internally.
