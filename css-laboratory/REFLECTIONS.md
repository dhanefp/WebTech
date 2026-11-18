# CSS Fundamentals Laboratory: Reflections

## Laboratory 1

**What is the difference between inline, internal, and external CSS?**

- **Inline CSS** goes directly on one element with the `style` attribute. It affects only that element.
- **Internal CSS** sits inside a `<style>` tag in the page's `<head>`. It affects only that one page.
- **External CSS** lives in a separate `.css` file connected with a `<link>` tag. Any page that links to it can use it.

**Which method would you use for a website with multiple pages? Explain why.**

External CSS. One stylesheet can style every page, so a single change (like a new heading color) updates the whole site at once. It keeps the HTML clean and the design consistent, and the browser can cache the file so pages load faster.

## Laboratory 2

**Explain the difference between `.card` and `#page-title`.**

`.card` is a class selector. A class can be used on many elements, so all three cards share the same style. `#page-title` is an ID selector. An ID must be unique and appear only once per page, so it targets one specific element. IDs also have higher priority (specificity) than classes when both style the same element.

## Laboratory 4

**How does padding differ from margin?**

Padding is the space inside an element, between its content and its border. It takes on the element's background color. Margin is the space outside the border that pushes other elements away. It is always transparent.

**What does `box-sizing: border-box` do?**

It makes the `width` and `height` include the padding and border. A card set to `width: 280px` stays 280px wide no matter how much padding or border you add. Without it, padding and border are added on top, so the box grows bigger than expected.

**How can excessive margin affect a layout?**

Too much margin wastes space and pushes elements apart. It can force items onto new lines, cause horizontal scrolling on small screens, and make related content look disconnected.

## Laboratory 5: Observations

- **Resizing the browser:** `flex-wrap: wrap` moves cards to a new row when there isn't enough room for each card's 220px base width.
- **`justify-content: space-between`:** the first card touches the left edge, the last touches the right edge, and the leftover space is split between them.
- **`align-items: center` vs `stretch`:** `stretch` makes all cards the same height as the tallest one. `center` lets each card keep its natural height and lines them up through the middle.
