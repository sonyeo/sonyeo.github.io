---
title: SwiftUI re-rendering
description: A reference page in my new Starlight docs site.
---

Reference pages are ideal for outlining how things work in terse and clear terms.
Less concerned with telling a story or addressing a specific use case, they should give a comprehensive outline of what you're documenting.

## Further reading

- Read [about reference](https://diataxis.fr/reference/) in the Diátaxis framework

## 이미지 테스트
한글 테스트  
![alt text](../../../assets/swiftui/swiftui_rerendering/디맥.png)

잘 되나?
```swift
Task.detached { // Task.detached 메서드 호출
    await doSomething()
}

- let detachedTask = Task.detached(priority: .medium) {
-     await doSomething()
- }
+ if (!detachedTask.isCancelled) {
+     detachedTask.cancel()
+ }
```