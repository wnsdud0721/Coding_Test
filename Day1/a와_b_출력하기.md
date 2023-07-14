## ✅ a와 b 출력하기
```swift
import Foundation

let n = readLine()!.components(separatedBy: [" "]).map { Int($0)! }
let (a, b) = (n[0], n[1])

print("a =",a)
print("b =",b)
// print("a = \(a)\nb = \(b)")
```
- \(값) 를 이용하여 외부의 값을 가지고 올 수 있음
- \n 은 줄바꿈
