# Base58

[![Platform](https://img.shields.io/badge/Platforms-macOS%20%7C%20iOS-blue)](#platforms)
[![Swift Package Manager compatible](https://img.shields.io/badge/SPM-compatible-orange)](#swift-package-manager)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/anquii/Base58/blob/main/LICENSE)

An implementation of [Base58](https://en.bitcoinwiki.org/wiki/Base58) in Swift. All credit goes to [keefertaylor](https://github.com/keefertaylor) for publishing the implemention [here](https://github.com/keefertaylor/Base58Swift), and to [a2hill](https://github.com/a2hill) for fixing [this](https://github.com/keefertaylor/Base58Swift/issues/18) issue.

## Platforms
- macOS 10.15+
- iOS 13+

## Installation

### Swift Package Manager

Add the following line to your `Package.swift` file:
```swift
.package(url: "https://github.com/anquii/Base58.git", from: "1.0.0")
```
...or integrate with Xcode via `File -> Swift Packages -> Add Package Dependency...` using the URL of the repository.

## Usage

```swift
import Base58

let base58: Base58Coding = Base58()
let encodedString = base58.encode(data: data)
let decodedData = try base58.decode(string: encodedString)
```

## License

`Base58` is licensed under the terms of the MIT license. See the [LICENSE](LICENSE) file for more information.
