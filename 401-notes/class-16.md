## Class 16 Notes

1. **What are the key characteristics of serverless computing, and how does it differ from traditional server-based architectures?**

    - [Serverless Computing](https://www.ibm.com/topics/serverless):

        - **No Server Management:** You don't need to provision or maintain servers, the cloud provider does it all for you, chosen undead.

        - **Automatic Scaling:** Automatically scales the application by adjusting the capacity, if you see more volume than usual, it'll adjust itself to accomodate that.

        - **Cost-Effective:** You pay only for the resources you consume, often measured in terms of the runtime of the code or the number of executions.

        - **Statelessness:** Serverless functions are stateless, meaning each execution is independent.

    - Traditional Server-Based Architectures:

        - **Server Management Required:** Requires setting up and managing servers, either physically or virtual servers in the cloud.

        - **Manual Scaling:** Scaling requires manual intervention to provision additional servers or resources.

        - **Continuous Costs:** Costs are ongoing for server maintenance and operation, regardless of the usage.

2. **How can one get started with Vercel, and what are the main steps involved in deploying a serverless function using Vercel?**

    [Steps to Deploy a Serverless Function using Vercel](https://vercel.com/docs/getting-started-with-vercel):

    1. **Sign Up/Login:** Create a Vercel account or log in if you already have one.

    2. **Install Vercel CLI:** Download and install the Vercel Command Line Interface (CLI) on your local machine.

    3. **Create a Project:** Start a new project. This can be done using a template or by initializing a new project in a supported framework.

    4. **Develop Your Function:** Write your serverless function code. This could be in JavaScript, Python, or other supported languages.

    5. **Configure Deployment:** Set up vercel.json to configure deployment settings, routes, and environment variables.

    6. **Deploy:** Use the Vercel CLI to deploy your project. Run a command like vercel to deploy your application.

    7. **Testing and Access:** Once deployed, test your serverless function via the provided URL and make any necessary adjustments.

    Source: ChatGPT

3. **What are APIs, and how can they be utilized in Python applications to access and manipulate data from external sources?**

- [API](https://realpython.com/python-api/)

    - APIs are sets of protocols and tools that allow different software applications to communicate with each other.
    - They enable your application to interact with external services or data sources.
    - You can access and manipulate data similar to Javascript in which you use the req and res such as POST, GET etc.

4. **What is the Requests library in Python, and how can it be used to interact with APIs by sending HTTP requests? Can you provide an example of a basic GET request using the Requests library?**

    - The Requests library in Python simplifies HTTP requests. It's user-friendly and can handle various types of HTTP requests (GET, POST, PUT, DELETE, etc.).

```
import requests

# URL of the API endpoint
url = 'https://api.example.com/data'

# Make a GET request
response = requests.get(url)

# Print the status code and response data
print(f"Status Code: {response.status_code}")
print(f"Response Content: {response.content}")
```