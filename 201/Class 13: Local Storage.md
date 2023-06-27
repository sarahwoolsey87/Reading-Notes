# Local Storage

[Local Storage & How to Use it on Websites](https://www.smashingmagazine.com/2010/10/local-storage-and-how-to-use-it/)

## Why would a developer use local storage for a web application?

- **Persistent Data Storage:** Local storage provides a way to store data on the client-side that persists even when the browser is closed. This can be useful for applications that need to remember user preferences, settings, or state between visits.

- **Offline Capability:** Local storage allows web applications to work offline by storing essential data locally. This enables users to access certain features or content even when they are not connected to the internet.

- **Performance Improvement:** Storing data in local storage can reduce the need for frequent server requests, improving the performance of the application. Instead of fetching the same data repeatedly, it can be retrieved from local storage, resulting in faster response times.

## What information should not be stored in local storage?

- **Sensitive Data:** Local storage is not secure and should not be used to store sensitive information such as passwords, credit card details, or personally identifiable information (PII). Storing such data in local storage can make it vulnerable to unauthorized access or theft.

- **Critical Application Data:** Local storage should not be relied upon for storing critical application data that is necessary for the proper functioning of the application. If the data is lost or corrupted in local storage, it could lead to a degraded user experience or even application errors.

## Local storage can store what type of data? How would you convert it to that type before storing?

> Local storage can store data in the form of strings. To store data of other types, such as objects or arrays, it needs to be converted to a string representation using a process called serialization. The two common methods for serializing data are:

- **JSON.stringify():** This method converts JavaScript objects or arrays into a JSON string representation, which can be stored in local storage.

- **toString():** For simple data types like numbers or booleans, they can be converted to strings using the toString() method before storing in local storage.

> When retrieving data from local storage, the opposite process called deserialization is used to convert the stored string back into its original data type:

- **JSON.parse():** This method is used to parse a JSON string stored in local storage and convert it back into a JavaScript object or array.

- **Parsing Functions:** For simple data types, parsing functions like parseInt() or parseFloat() can be used to convert the string representation back to the original data type.

[The Past, Present & Future of Local Storage for Web Applications](http://diveinto.html5doctor.com/storage.html)