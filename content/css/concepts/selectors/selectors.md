---
Title: 'Selectors'
Description: 'Selectors are used to style HTML elements according to their type and/or attribute(s).'
Subjects:
  - 'Web Development'
  - 'Web Design'
Tags:
  - 'Selectors'
  - 'Elements'
  - 'Style'
CatalogContent:
  - 'learn-css'
  - 'paths/front-end-engineer-career-path'
---

**Selectors** are used to style [HTML elements](https://www.codecademy.com/resources/docs/html/elements) according to their type and/or attributes.

All markups can be selected with the `*` selector:

```css
* {
  /* declarations here */
}
```

## Selecting by Type

The element selector selects HTML elements based on the element name.

### Syntax

```css
element-name {
  /* declarations here */
}
```

The `element-type` must be a valid HTML element.

### Example

In the following example, all `<p>` elements on the page will be center-aligned, with a red text color:

```css
p {
  text-align: center;
  color: red;
}
```

## Selecting by Attribute

Most commonly, the `class` and `id` attributes are assigned to elements for styling purposes. An `id` cannot start with a number.

### Syntax

```css
#id-name {
  /* declarations here */
}

.class-name {
  /* declarations here */
}

element[attribute='value'] {
  /* declarations here */
}
```

The `id` of an element is unique within a page, so the `id` selector is used to select one unique element. An element can be selected with a specific `id`, by using a hash (`#`) character, followed by `id-name`.

Multiple `class` values can be assigned to a single element. Elements are selected by `class` with a period (`.`) character, followed by `class-name`. Unlike `id` values, `class` values can be duplicated on a page with different elements.

### Example

The following rules select elements based on `id`, `class`, and other attributes:

```css
#para1 {
  text-align: center;
  color: red;
}

.center {
  text-align: center;
  color: red;
}

li[title='red'] {
  background-color: red;
  color: #fff;
}
```

It can also be specified that only certain HTML elements with a given class should be styled. For example, here, only `<p>` tags with a `class` of `"center"` will have its text center-aligned:

```css
p.center {
  text-align: center;
  color: red;
}
```

## Video Walkthrough

Watch this video on how to compare the various selectors in CSS.

<iframe width="560" height="315" src="https://www.youtube.com/embed/Xv6KmV2Zp4c" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
