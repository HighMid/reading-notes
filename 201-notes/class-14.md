## Class 14 Notes

### CSS Transforms

1. **What does a CSS transform allow the developer to do to an element?**

    > CSS transform allows you to change the shape, size, position and orientation of an element in a two-dimensional or three-dimensional space.  These can be used for many visual effects like rotating, scaling or moving elements.

2. **Provide an example of a transform and how you could see that being used on a website.**

    - Below this will rotate the element 45 degrees clockwise,
    ```
    .rotate-element {
    transform: rotate(45deg);
    }
    ```


### CSS Transitions & Animations

1. **What does a CSS transition allow the developer to do to an element?**

    > CSS Transitions allows you to change property values smoothly over a specified duration.  Changes happen gradually over a period of time which can result in a smoother and visually appealing effect.

2. **How does a CSS animation differ from a CSS transition?**

    - **Complexity and Control**: CSS animations are more powerful and provide more control than transitions. With animations, you can define keyframes to control the intermediate steps of the animation sequence, allowing for more complex sequences than the start and end states used in transitions.

    - **Triggering the Effect**: Transitions are typically triggered by a change in a CSS property value, such as on hover or on focus. Animations, on the other hand, can run independently of a state change. They can start as soon as the page loads or be triggered by JavaScript.

    - **Repetition and Timing**: Animations can be set to repeat indefinitely or a specific number of times, and they allow for more control over timing and delays. Transitions generally occur only once (like when a state changes) and don't have built-in repetition without additional JavaScript.

    - **Syntax:** Animations require defining keyframes using the @keyframes rule, where you specify the styles at various points during the animation. Transitions, in contrast, are simpler, requiring only the specification of the property to transition, the duration, the timing function, and optionally, a delay.
    **Source:ChatGPT**

3. **What are some benefits to using CSS transitions on websites?**

    - Helps make the website more aethesically pleasing to users which is crucial for engagement as your typical user will take about 10 seconds to determine whether or not the website is of interest.

    - They also can guide users with subtle hints to direct attention to certain areas of the webpage such as changes to content when posed too or just emphasizing important details.

4. **How this topic fit in with your long-term goals?**

    > It'll help for me because I like making webpages that can tell a story, every bit of motion has a purpose and this can help achieve that.  On top of helping performance optimization and creative expression this these transitions/animations will have a big impact on me if I ever make a webpage for myself.

### Psychological Safefy

1. **What are three key factors that contribute to psychologically safe teams?**

    - Interpersonal Trust and Mutual Respect: Team members feel safe to take risks and be vulnerable in front of each other.
    - Openness and the Ability to Speak Up: An environment where individuals feel they can voice their opinions and ideas without fear of punishment or humiliation.
    - Diversity and Inclusiveness: A setting where diverse perspectives are valued and contribute to the team's success.

2. **Evaluate, with details, a previous professional setting (or team) you were in with regards to psychological safety.**

    > Won't go into details but an event I had in the military essentially made me realize that my supervisors who were suppose to help guide the Junior enlisted were both ego tripping losers. The environment was pretty hostile and you already know it's bad when they start to introduce mandatory fun.  Voiced concerned were glossed over and most of those people(included myself) got isolated for job upgrades, potential TDYs etc.

3. **What impact do teams that operate with a high degree of psychological safety have on their company and the team members?**

    - Teams with high psychological safety are typically more productive, innovative, and collaborative.  

    - They contribute positively to the company by driving performance and employee engagement.

    - Team members in such environments are likely to have higher job satisfaction, contribute more freely, and have a stronger commitment to the team and company goals.
