## Class 34 Notes

1. **What are the key principles to follow when organizing and configuring Django settings for a project, according to the “Django Settings Best Practices” reading?**

    - Django Best practices seem to follow along with just ANY sort of practice regarding projects and version control,

        - Store critical pieces of information in `.env` and ensure that any variables or settings that require it are secured when set to production

        - Version control is important, in case something unprescented happens and you are required to revert back to an earlier working version. 

            - Also fun fact, just in case someone decides to screw you over if you're working on a collaborative project, fork the repo you are working on or maintain your local copies. Local copies are good but forking a project allows you to keep your contributions to the repo and in the event the base repo is gone you'll still have your copy.

        - Use different settings for different environments, you should have settings for production and for development. This helps clear the distinction between the two and allows for less mistakes to happen as the proper settings should be bundled correctly in accordance to the current stage.

2. **How does the White Noise library contribute to the efficient serving of static files in a Django application, and what are the steps to integrate it into a project?**

    - The White Noise library simplifies the process of using static files for deployment but making it unreliant on external services.
        - This also improves the performance as these can be cached to speed loading times of returning users and also compresses the files.
    
    - White noise library can be implemented by:

        1. **Install White Noise:** Add White Noise to your project using pip: `pip install whitenoise`.

        2. **Configure Middleware:** Add White Noise's middleware to your MIDDLEWARE settings in `settings.py`, ideally right after django.`middleware.security.SecurityMiddleware`:

        ```
        MIDDLEWARE = [
            'django.middleware.security.SecurityMiddleware',
            'whitenoise.middleware.WhiteNoiseMiddleware',
        ]
        ```

        3. **Serve Static Files:** Configure your static files settings (`STATIC_URL` and `STATIC_ROOT`) and use `collectstatic` to collect static files in your chosen directory. White Noise will serve these files directly in production.

3. **What is the purpose of Cross-Origin Resource Sharing (CORS) in web applications, and how can it be implemented and configured in a Django project to control access to resources?**

    - CORS is back and quite frankly I would send it my birthday card invitation. CORS is a security feature that restricts access to certain web pages from making requests to a different domain than the served web page. This prevents malicious websites on making requests to another site essentially impersonating the user.

    - CORS can be implemented by,

        1. **Install Django CORS Headers:** Use pip to add the `django-cors-headers` library to your project: `pip install django-cors-headers`.

        2. **Configure Middleware:** Add `corsheaders.middleware.CorsMiddleware` to your `MIDDLEWARE` setting in `settings.py`, ideally as high as possible, especially before any middleware that can generate responses:

        ```
        MIDDLEWARE = [
            'corsheaders.middleware.CorsMiddleware',
        ]
        ```

        3. **Configure Allowed Origins:** Use `CORS_ALLOWED_ORIGINS` in `settings.py` to specify which origins are allowed to make cross-origin requests to your Django backend:

        ```
        CORS_ALLOWED_ORIGINS = [
            'http://localhost:3000',
            'https://example.com',
        ]
        ```

