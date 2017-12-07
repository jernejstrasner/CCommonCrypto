# CCommonCrypto

This is a CommonCrypto SPM (Swift Package Manager) Package that allows for linking to CommonCrypto. It contains a modulemap file and CommonCrypto headers. The latter is because the headers are not available in a general path – instead they are part of the Xcode bundle and thus not very portable.

# Usage

```swift
let package = Package(
    name: "YourPackage",
    dependencies: [
        .package(url: "https://github.com/jernejstrasner/CCommonCrypto.git", .branch("master"))
    ],
    targets: [...]
)
```
