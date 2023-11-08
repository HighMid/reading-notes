## Class 13 Notes

### Local Storage and usage on Websites

1. **Why would a developer use local storage for a web application?**

    - Provides a way to access data locally such as user preferences, game data or other types of data that is helpful to have across other visits.

    - Less server requests as data saved locally does not need to be retrieved multiple times from the server.

    - Usage during different network conditions such as offline accessibility.

2. What information should not be stored in local storage?

    - Sensitive information such as PII, HIPA, etc. should not be stored locally as it is not secure.

    - Local storage is not encrypted and can be accessed by any script in the page.

3. Local storage can store what type of data? How would you convert it to that type before storing?

    - Local storage is only capable of storing strings therefore any data type other than strings must be converted before storing.

    - You are able to convert data to strings using `JSON.stringify()` *(I would love to be in a position to make a method named that)*

    >- Converts to a String
    ```
    let data = { name: "John", age: 30 };
    localStorage.setItem("userData", JSON.stringify(data));
    ```

    >- Converts back to an object or array
    ```
    let dataString = localStorage.getItem("userData");
    let data = JSON.parse(dataString);
    ```