## Placeholder File

1. **What are the key differences between scraping static and dynamic websites?**

    1. **Content Delivery**:

        - **Static Websites**: The content is fixed and served directly from the server as HTML. It does not change unless the HTML file is updated on the server.

        - **Dynamic Websites**: The content is dynamically generated, often depending on user interaction or other variables. It often involves client-side scripting (JavaScript) to fetch data, usually from APIs, after the initial HTML is loaded.

    2. **Scraping Methodology**:

        - **Static Websites**: Can typically be scraped using simple HTTP requests to download the HTML content, as the content is readily available in the initial HTML response.

        - **Dynamic Websites**: Often require rendering JavaScript and making additional HTTP requests that are triggered after the page is loaded. Tools like Selenium, Puppeteer, or Playwright are needed to execute JavaScript and fetch dynamically loaded content.

    3. Complexity and Resources:

        - **Static Websites**: Easier to scrape and less resource-intensive since it’s mostly about parsing HTML.

        - **Dynamic Websites**: More complex and resource-intensive as it involves rendering pages, executing JavaScript, and possibly dealing with AJAX calls.

    Source: ChatGPT

2. **Explain at least three techniques or best practices that can be employed to avoid getting blocked while scraping websites.**

    1. Robots.txt - Check and adhere to the `robots.txt` file of the website, this will tell you the site's scraping policy

    2. Agent Rotation - Use different use-agent strings to avoid being branded a bot, this helps in mimicing normal user traffic.
    
    3. Rate Throttling - Use delays to avoid hitting servers too frequently, this also helps mimic normal user interactions.

    - Honorable Mentions
        - Captcha Solving Services: This is my favorite suggestion, using third party services to essentially bypass captcha.

        - IP rotating: Using proxy servers or VPNs to change your IP to avoid IP bans, this isn't so bad as generally being on a VPN isn't exactly abnormal

3. **What is Playwright, and how does it assist in web scraping tasks? Provide an example of a use case where Playwright would be particularly beneficial.**

    - Playwright is an open-source automation library that allows for browser automation that supports multiple languages and provides APIs to automate web browser interactions.

    - An example would be interactive websites that require interaction such as clicks and form submissions, Playwright can be used to interact with these pages.

4. **Describe the purpose of using Xpath in web scraping, and provide an example of an Xpath expression to select a specific HTML element from a webpage.**

    - Xpath is used to navigate through elements and attributes in an XML document.
        - This allows for precise selection of elements, attributes within the HTML document, expressions can be used to navigate the HTML tree structure.

```
# Selecting all the links in the `<a>` tags within a `div` with an `id` of content
//div[@id='content']/a
```