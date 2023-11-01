## Class 08 Notes

### Flexbox

1. **Flexbox is designed for one-dimensional content. Explain what this means.**

    >- Flexbox lays out items in a single row/column but not at the same time.  It's because it can only do one or the other is why it's powerful for specific layouts regarding rows or columns.

2. **Explain the difference between the main axis and cross axis.**

    - **Main Axis** - is the primary axis in which flex items are laid out.  The direction is determined by `flex-direction`, this can be set to either `row` or `column`.
    - **Cross Axis** - cross axis is perpendicular to the main axis so if the main axis runs vertically (`column`), it'll run horizontally and vice versa.

3. **How can using certain properties of flexbox negatively impact accessibility?**

    >- `order` is a property that allows the reordering of items in groups. This makes changes to the screen visually however users who use assistive devices such as screen readers will read out the source.  It's better practice to adjust the source other than using this to visually change something unless it's intended to be that way.

4. **What are some advantages of using flexbox over float?**

    - Flexbox is easier and cleaner: When using float, you often need to clear the float, which can be a hassle. With flexbox, there's no need to clear anything.

    - Flexbox is more predictable: Float can sometimes behave unpredictably, especially when you have elements of varying heights. Flexbox gives you more control over your layout.

    - Alignment and distribution: Flexbox provides properties like justify-content and align-items which make it easier to align and distribute items within a container.

    - Flexbox is more flexible: As the name suggests, flexbox is inherently more flexible and adaptable to various screen sizes and devices. This makes it a great choice for responsive design.

    - Direction agnostic: Flexbox doesn't care if your layout is horizontal or vertical, and you can switch between them with ease.

5. **How does this topic connect with your long term goals?**

    > Truthfully if my goal was to be a web developer then hell yeah, using and understanding flexbox is really nice as it's a powerful tool to be using.  It seems to snuff out a lot of the nuances of using `float` and in the experiences I have with it the last two days, proven very useful in providing clean looking layouts.  Now if I didn't suck so bad with CSS at the moment then maybe I would be super excited to play around with flexbox more but yeah maybe one day.