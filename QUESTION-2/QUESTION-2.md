In CSS (Cascading Style Sheets), "absolute" and "relative" are terms used to describe positioning properties. They determine how an element is positioned within its containing element or the document flow. Here's the difference between absolute and relative positioning:

1. **Relative Positioning:**
   - When an element is set to `position: relative;`, it is positioned relative to its normal position in the document flow.
   - If you apply additional positioning properties like `top`, `right`, `bottom`, or `left`, they will be calculated relative to the element's original position.
   - Other elements in the document flow are not affected by the relative positioning of the element.

   ```css
   .relative-box {
     position: relative;
     top: 20px;
     left: 30px;
   }
   ```

2. **Absolute Positioning:**
   - When an element is set to `position: absolute;`, it is positioned relative to its nearest positioned (not static) ancestor, if any. If no such ancestor exists, it is positioned relative to the initial containing block, which is usually the `<html>` element.
   - Absolute positioning takes the element out of the normal document flow, meaning it does not affect the layout of other elements, and other elements do not affect its position.
   - If you apply additional positioning properties, they are calculated relative to the nearest positioned ancestor.

   ```css
   .absolute-box {
     position: absolute;
     top: 50px;
     left: 100px;
   }
   ```

