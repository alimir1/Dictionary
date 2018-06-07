# Dictionary

[![](https://img.shields.io/badge/Swift-4.0-orange.svg?style=flat-square)](https://developer.apple.com/swift/ "Swift 4") ![](https://img.shields.io/badge/platform-macOS,%20iOS-yellowgreen.svg?style=flat-square "Platform: macOS, iOS") [![](https://img.shields.io/badge/license-MIT-lightgrey.svg?style=flat-square "License: MIT")](LICENSE.md)

**Dictionary** is a lightweight Swift library to perform word searches in a dictionary.
<br />
<br />
**Author:** Ali Mir<br />
**Date:** June 7, 2018<br />

## Requirements

- Swift 4
- Xcode 9+

# Installation
Simply drag [`Dictionary.swift`](/Dictionary.swift) to your project.

# Usage
```SWIFT
let dict = Dictionary()
print(dict.words(with: "animal"))
// => ["animality", "animallike", "animalistic", "animalculum", "animalcules", "animalist", "animalizing", "animalizes", "animalcule", "animalism", "animals", "animally", "animalization", "animalize", "animalcula", "animal", "animalized"]
print(dict.isValid(word: "animal"))
// => true
print(dict.isValid(prefix: "joe"))
// => true
```

## Notes
This library uses a [Trie](https://en.wikipedia.org/wiki/Trie) (aka Prefix Tree) internally.
