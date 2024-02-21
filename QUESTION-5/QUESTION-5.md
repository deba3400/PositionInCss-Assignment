In CSS, the `z-index` property is used to control the stacking order of positioned elements on a web page along the z-axis (depth). It determines which elements are shown in front of or behind others when they overlap. The element with a higher `z-index` value will appear in front of elements with lower values.

The `z-index` property can take numerical values, including negative values, and is typically applied to positioned elements (those with a `position` property value other than `static`, such as `relative`, `absolute`, or `fixed`).

Here's a simple example:

```css
.element1 {
  position: relative;
  z-index: 2;
}

.element2 {
  position: relative;
  z-index: 1;
}
```

In this example, `element1` will appear in front of `element2` because it has a higher `z-index` value. Keep in mind that the `z-index` property only affects elements that are positioned, so if an element does not have a `position` value other than `static`, the `z-index` property will have no effect.

It's important to use `z-index` judiciously and avoid excessive use of high values, as it can make the code harder to maintain and understand. Additionally, keep in mind that the `z-index` property only works on positioned elements within the same stacking context.