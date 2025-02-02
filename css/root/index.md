---
title: "`:root`"
authors:
  - lenaryan
editors:
  - tachisis
keywords:
  - :root
  - псевдокласс
  - кастомные свойства
  - переменные
tags:
  - doka
---

## Кратко

Псевдокласс `:root` нужен для обращения к самому главному родительскому элементу документа. Его также называют корневым элементом. В случае HTML-документа самым главным родителем всей страницы будет тег `<html>`. Часто `:root` используется для того, чтобы задавать [кастомные свойства](/css/custom-properties).

## Пример

Укажем в документе нужный нам шрифт и создадим несколько кастомных свойств:

```css
:root {
  font-family: 'Oswald', sans-serif;
  --button-size: 40px;
  --main-color: #bada55;
}
```

## Как пишется

Пишется, как обычный псевдокласс: после двоеточия пишем слово root. Однако в отличие от других псевдоклассов `:root` полностью самостоятельный, его не используют в связке с другими селекторами.

## Как это понять

Корневой элемент — это самая главная обёртка в документе, самый первый родитель. В HTML-документах псевдокласс `:root` будет ссылаться на тег [`<html>`](/html/html). Поскольку CSS работает ещё и в SVG-, и XML-файлах, для них корневой элемент будет другим. В SVG-документах родителем будет тег `<svg>`, а в XML-документах — тег `<xml>`.
