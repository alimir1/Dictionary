# Dictionary

[![](https://img.shields.io/badge/Swift-4.0-orange.svg?style=flat-square)](https://developer.apple.com/swift/ "Swift 4") ![](https://img.shields.io/badge/platform-macOS,%20iOS-yellowgreen.svg?style=flat-square "Platform: macOS, iOS") [![](https://img.shields.io/badge/license-MIT-lightgrey.svg?style=flat-square "License: MIT")](LICENSE.md)

**Dictionary** is a lightweight Swift library to perform word searches in a dictionary.
<br />
**Author:** Ali Mir<br />
**Date:** June 7, 2018<br />

## Requirements

- Swift 4
- Xcode 9+

# Installation
Simply drag [`Dictionary.swift`](/Dictionary.swift) to your project.

# Usage
Create an instance of `Dictionary`.<br />
`words(with prefix: String)` - returns all words with given prefix<br />
`isValid(word: String)` - A Boolean that indicates if a given String is a valid word in the English dictionary.<br />
`isValid(prefix: String)` - A Boolean that indicates if a given String is a valid prefix in English dictionary.<br />
```SWIFT
let dict = Dictionary()
print(dict.words(with: "animal"))
print(dict.isValid(word: "animal"))
print(dict.isValid(prefix: "joe"))
```

## Notes
This library uses a [Trie](https://en.wikipedia.org/wiki/Trie) (aka Prefix Tree) internally.
