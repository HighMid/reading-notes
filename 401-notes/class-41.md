## Class 41 notes

1. **Explain the concept of dynamic routes in Next.js and how they differ from static routes.**

    - **Static Routes:**

        - Static routes are the most basic type of route in Next.js. They directly map to a file in the pages directory. For example, the file pages/about.js would automatically be accessible via the /about URL. These routes are known at build time and do not change unless the developer updates the application.

        - They are straightforward and ideal for pages whose content does not depend on external data sources or user input.

    - **Dynamic Routes:**

        - Dynamic routes allow you to create pages that can handle a variety of paths, often based on data. These are defined by adding square brackets to a page's filename, such as `[id].js` within the pages directory. This tells Next.js that this is a dynamic page, where the part of the URL enclosed in brackets is variable.

        - They are essential for when you want to create pages based on external data sources, like a database or API. For example, if you're building a blog, you might have a dynamic route for blog posts that looks like /posts/[slug], where each post's slug determines which specific post to render.

        - The difference lies in flexibility and data dependence. Dynamic routes can adapt to different data inputs, allowing for more complex and interactive applications.

2. **Describe the process of deploying a Next.js application. What are the key steps involved, and what are some deployment platforms you can use?**

    - **Build Your Application:** Run the next build command. This command generates the .next directory with all the files needed for production.

    - **Choose a Hosting Provider:** There are several platforms suited for Next.js applications, such as Vercel (the creators of Next.js), Netlify, and AWS Amplify. Each platform has its own set of features and deployment process.

    - **Configure Your Application for Deployment:** Depending on your hosting provider, you might need to configure some settings, such as environment variables, build commands, or publish directories. For Vercel, this can be as simple as linking your GitHub repository and setting up automatic deploys.

    - **Deploy Your Application:** This step varies by platform. If you're using Vercel, pushing your code to GitHub can automatically trigger a deployment. For other platforms, you might need to use their CLI or web UI to deploy your application.

    - **Monitor and Update:** Once deployed, use your platform's tools to monitor your application's performance and health. Update your application as needed by pushing new code, which can often trigger a new deployment.

3. **How does Next.js handle static file serving? Discuss the default folder structure for storing static assets and explain how to reference them in a Next.js application.**

    - Default Folder Structure: Place your static assets in the public directory. For example, if you add an image at public/images/my-image.png, you can reference it in your Next.js application via /images/my-image.png.

    - Referencing Static Assets: In your Next.js components, reference these assets using a relative path from the root of the public directory. For example, using an `<img>` tag to display an image would look like this: 

    ```
    <img src="/images/my-image.png" alt="My Image">.
    ```