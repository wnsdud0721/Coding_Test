## ✅ flag에 따라 다른 값 반환하기

### ❓문제
- 입력값: -4, 7 , true / -4, 7, false
- 기댓값: 3 / -11

### ❗️1번 풀이
```swift
import Foundation

func solution(_ a:Int, _ b:Int, _ flag:Bool) -> Int {
    return flag ? a + b : a - b
}
```
