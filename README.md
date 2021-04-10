# CGPointVector

[![CGPointVector CI](https://github.com/koher/CGPointVector/actions/workflows/tests.yml/badge.svg)](https://github.com/koher/CGPointVector/actions)

_CGPointVector_ provides the extension for arithmetic operations with _CGPoint_ in __Swift__, which are convenient when _CGPoint_ values are used as vectors.

```swift
let a = CGPoint(x: 1, y: 2), b = CGPoint(x: -3, y: 5)

let sum = a + b // (-2.0, 7.0)
let distance = (b - a).length // 5.0
let direction = (b - a).unit // (-0.8, 0.6)
let rotated = a * CGAffineTransform(rotationAngle: CGFloat.pi / 2) // (-2.0, 1.0)
```

## Usage

```swift
import CGPointVector

let a = CGPoint(x: 3.0, y: -4.0)
let b = CGPoint(x: 2.0, y: -5.0)

let sum = a + b // (5.0, -9.0)
let length = a.length // 5.0
let distance = a.distance(from: b) // 1.4142135623731
let unitVector = a.unit // (0.6, -0.8)
let dotProduct = a.dot(b) // 26.0
let angle = a.angle(from: b) // 0.26299473168091936
```

## License

[The MIT License](LICENSE)
