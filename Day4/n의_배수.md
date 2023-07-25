
## ✅ n의 배수

### ❓문제
- 입력값: num =. 8, n = 2 / num = 34, n = 3
- 기댓값: 1 / 0

### ❗️1번 풀이
```swift
import Foundation

func solution(_ num:Int, _ n:Int) -> Int {
    return num % n == 0 ? 1 : 0
}
```

### ❗️2번 풀이
```swift
import Foundation

func solution(_ num:Int, _ n:Int) -> Int {
    return num.isMultiple(of: n) ? 1 : 0
}
```
[isMultiple(of:) | Apple Developer Documentation](https://developer.apple.com/documentation/swift/int/ismultiple(of:))
- isMultiple(of:)는 배수인지 판단하는 메서드
- isMultiple(of:)와 % 연산자의 차이
    1. 0으로 나누는 상황에서 number % 0 == 0 은 무조건 True. 하지만 number.isMultiple(of: 0)은 number가 0이면 True, 아니라면 False
    2. 오버플로우에 대한 표현 차이
        - signed integer인 T에 대해 T.min.isMultiple(of: -1)은 True
        - T.min / -1은 오버플로우로 인해 컴파일 에러가 발생
