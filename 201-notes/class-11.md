## Class 11 Notes

### Video and Audio Content

1. **Explain how the ability to use video and audio on the web has evolved since the early 2000s.**

    > How we interact with videos and audio is vastly different now compared to the early 2000s. It may not seem that different on the surface but videos or audio files were embedded using Adobe Flash, Microsoft's Silverlight or Apple's Quicktime. I remember Flash being one of the go-to plugins used for games or videos online and even playing popular games like Runescape.  These plugins weren't however standized between browsers and had a lot of security risks (I lost many accounts on Runescape . . .), these plugins were superceded by HTML5 which allowed  embed media without the need for external plugins.

2. **Describe the use of the src and controls attributes in the `<video>` element.**

    > `<video>` uses the `src` attribute to specify the path to the video file that needs to be played.  It's what gives the `<video>` element to find the file in question.  `controls` is an attribute allows the user to control the video via playing, pausing, adjusting volumes and other actions if allowed.

3. **Why is it important to have fallback content inside the ``<video>`` element?**

    > It's important to have fallback content because it gives the user feedback in case the video isn't supported by the browser, the link is no longer valid or any message that gives user an idea on what the problem is.  These messages are important as this helps with web accessibility and a way to handle degradation.

4. **Write a very short story where `<audio>` and `<video>` are characters.**


    > In the digital town of Webville, two friends named `<audio>` and `<video>` lived harmoniously, sharing tales and songs with the locals. `<audio>`, with her melodious voice, would fill the air with podcasts and music, bringing soundtracks to life. `<video>`, with his vivid portrayals, would show the townsfolk movies and clips, painting stories in motion.

    >One day, a silence fell over Webville as a thick fog of Compatibility Issues rolled in. `<audio>` tried to sing, but her voice was muffled. `<video>` attempted to display his colorful tales, but the screen stayed blank. The townsfolk were lost without their stories and songs.

    >Then, `<audio>` had an idea. She called upon her old friends, the `<source>` siblings, who could speak in multiple codecs, ensuring that no matter what, her voice could be heard. `<video>` did the same, inviting `<source>` to bring his stories in various formats. They also created Fallback Scrolls, ancient texts that provided guidance whenever the townsfolk couldn't hear `<audio>` or see `<video>`.

    >Thanks to their ingenuity, the fog lifted. The townspeople cheered as `<audio>`'s songs filled their days and `<video>`'s stories lit their nights once more. Together, they ensured that all could enjoy the wonders of Webville, regardless of the device or browser they used, and they all lived in harmony ever after.

    > **Source: ChatGPT**

### Grid

1. **How does Grid layout differ from Flex?**

    - Grid is two-dimensional meaning it can render both rows and column simultaneously which is ideal in large scale layouts.  Flex focuses on one-dimensional, so it's either rows or columns but not as the same time.  It's ideal to use flex in smaller scale layouts.

2. **Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.**

    - Grid Container: The element on which display: grid is applied. It serves as the parent of all grid items and defines the grid's tracks and the spaces between them (gutters).

    - Grid Item: The children (direct descendants) of the grid container. Each grid item is positioned within the grid by assigning it to a grid area defined by grid lines.

    - Grid Line: These are the dividing lines that make up the structure of the grid. They can be either vertical ("column grid lines") or horizontal ("row grid lines"). Grid lines are referenced when placing grid items and defining grid template areas.

### Responsive Images

1. **Besides making a site visually appealing across different screen sizes, why should developers make images responsive?**

    - Helps with accessibility and overall user experience, this can help with the layout staying consistent as possible so unexpected layout shifts are minimal.

    - Having smaller images helps with bandwidth as they load faster and help appropriate for smaller devices such as phones.

    - Contribute to search engine rankings as how fast a page loads helps in the ranking.

2. **Define the following `<img>` attributes `srcset` and `sizes`. Write an example of how they are used.**

    - `srcset:` Defines a set of images for the browser to choose from, based on device pixel ratio or viewport width.

    - `sizes:` Specifies image display sizes in different conditions to help the browser select an appropriate image from srcset.

3. **How is `srcset` more helpful for responsive images than CSS or JavaScript?**

    >`srcset` lets the browser decide the best image to load before rendering the page, which is more efficient than using JavaScript. CSS can't offer different resolution images based on device capabilities, while srcset can, leading to better performance without extra overhead.