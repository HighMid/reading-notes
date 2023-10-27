## Class 05 Notes

### HTML

1. **What is a real world use case for the alt attribute being used in a website?**
    > You should use `alt` when describing a picture for people who are unable to view the image or/and using screen readers.  This usage of the attribute would be beneficial to those individuals as it can be used to help paint the picture for them.

2. **How can you improve accessibility of images in an HTML document?**

    - Using the `alt` attribute to add description, using `figure` to also add captions to images which adds to the context on what the image is/used to portray.
    - Making images Scalable, i.e. making sure they scale appropriately to the users specifications.  A user on the phone has a smaller screen therefore how they view the webpage should be different than how a user on a computer would view it.
    - Implement fixed/absolute positioning if trying to make comparisons of images or trying to explain an image while having the user read through the text but still having the image visible to the reader.

3. **Provide an example of when the figure element would be useful in an HTML document.**

    > They teased a new character in one of the game's I play and I wanted to know who made the concept art and if they're doing anything in the image.  You can put a description on what the image is/what they're doing then have captions describing the character and who was responsible for the art.

4. **Describe the difference between a gif image and an svg image, pretend you are explaining to an elder in your community.**

    > Differences between a **GIF** and a **SVG** *(Scalable Vector Graphics)* is that a GIF is a slideshow image, kinda like classic animation.  It may look like a video however, it's treated like an image but because it's essentially just an image sequence it's of lower quality.  SVG's are images that retain all of their sharpness and qualities even if the image is made larger or smaller.

5. **What image type would you use to display a screenshot on your website and why?**

    >- For screenshots, a PNG (Portable Network Graphics) format is often recommended. Why? Because PNGs support lossless data compression. This means they can reproduce the sharpness and clarity of the original screenshot without losing any quality. Screenshots often have text, sharp edges, and uniform colors, and PNG handles these very well, ensuring that the text and details remain legible and clear.<div>
    **Source: ChatGPT**
    >- Why PNG over SVG? PNGs are more widely supported because not all browsers can render SVGs properly, now most people use the Browser Trio (Chrome, Safari, Edge)

### CSS

1. **Describe the difference between foreground and background colors of an HTML element, pretend you are talking to someone with no technical knowledge.**

    >- The background color is kinda like a medium/canvas, it's the color that is applied before you start coloring on top of it which is foreground colors.  If you think about how a book looks, you can say the pages is the background color and the text is the foreground color.

2. **Your friend asks you to give his colorless blog website a touch up. How would you use color to give his blog some character?**

    >- I would ask if they wanted to do a specific theme that they're trying to go for. Like if they were blogging about hiking/nature etc. then I would use colors that represent the earth like green and brown. If they wanted to be super edgy then red and black, it depends on what they are trying to portray to the audience on his blog. [The Color Theory](https://www.canva.com/colors/color-wheel/) , is also an amazing tool to use if you're unsure on what you want to do but want to have colors that compliment each other well.

3. **What should you consider when choosing fonts for an HTML document?**

    >- Legibility: Ensure that the font is easy to read. Scripted or decorative fonts can be hard to decipher, especially in long texts.
    >- Mood & Tone: Different fonts convey different emotions. A formal document might use a more traditional font, while a creative blog might use something more playful.
    >- Compatibility: Some fonts might not display correctly on all devices or browsers. It's essential to choose widely supported fonts or use web-safe font families.
    >- Number of Fonts: Don't use too many different fonts; it can make the page look chaotic. Usually, 2-3 (one for headings, one for body, maybe one for special highlights) is sufficient.<div>
    **Source: ChatGPT**

4. **What do font-size, font-weight, and font-style do to HTML text elements?**

    >- **Font-size**: Determines the size of the text, you can make it bigger or smaller depending on the content
    >- **Font-weight**: This controls the thickness of the text.  Typically using bolded text gives more emphasis or importance, weight makes this thicker. Lighter also makes texts more thin.
    >- **Font-style**: This adjusts the style of the text such as making it italic.

5. **What do font-size, font-weight, and font-style do to HTML text elements?**

    >- **letter-spacing**: This property controls the space between characters. If you want the characters in your h1 element to have a bit more breathing room, you'd increase the letter-spacing value.
    >- **word-spacing**: This controls the space between words. If the words in your h1 seem too close together, you can adjust this to space them out a bit more.
 