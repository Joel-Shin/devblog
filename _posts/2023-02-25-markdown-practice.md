---
layout: post
title:  "Markdown Practice"
date:   2023-02-25 14:02:25 +0900
categories: development 
---


## Heading 2

### Heading 3

#### Heading 4

---

## Bold Text

this is an example of **bold text**

## Italic Text

this is an example of *italicized text*

## Ordered List

1. number 1
2. number 2
3. number 4
4. number 4

## Ordered List 2

1. number 1
1. number 2
1. number 3
1. number 4
1. number 5

## Unordered List

- dot 1
- dot 2
- dot 3
  - nested dot 1
  - nested dot 2
  - nested dot 3
    - nested nested dot 1
    - nested nested dot 2

## Code Snippet

```swift
struct PositionObservingView<Content: View>: View {
    var coordinateSpace: CoordinateSpace
@Binding var position: CGPoint
    @ViewBuilder var content: () -> Content
    var body: some View {
        content()
            .background(GeometryReader { geometry in
                Color.clear.preference(
    key: PreferenceKey.self,
    value: geometry.frame(in: coordinateSpace).origin
)
            })
            .onPreferenceChange(PreferenceKey.self) { position in
                self.position = position
            }
    }
}
```

## Highlight Quotes

In this course we are going to use **ruby**, **kotlin**, **xml**.

In this course we are going to use `ruby`, `kotlin`, `xml`.

## Block Quotes

> "this is what someone famous once said" - someone famous

## URLs or Link

[this is to google](https://www.google.com)

## Images

![image](https://cdn.dribbble.com/userupload/4917004/file/original-5063c748bd20c441edd26c28f34654a8.jpg?compress=1&resize=1024x1024)

![image](https://res.cloudinary.com/dg8gqr85x/image/upload/v1677304520/sample_kxi3gt.png)

