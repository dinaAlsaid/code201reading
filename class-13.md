# Code 201

[PREVIOUS](https://dinaalsaid.github.io/code201reading/class-12) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)  &nbsp; [NEXT](https://dinaalsaid.github.io/code201reading/class-14)

## Local storage

If the web application needs more storage than key/value pairs you can embed a database.

why not use cookies to store data?

* Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over.
* Cookies are included with every HTTP request, thereby sending data unencrypted over the internet
* Cookies are limited to about 4 KB of data — enough to slow down your application, but not enough to be terribly useful.

what we want is a lot of storage on the client side and data to not b tramsitted to the server.

Before HTML5, people used userData that allowed web pages to store up to 64+ KB of data per domain, in a hierarchical XML-based structure, that was developed by microsoft for Internet Explorer, and many other solutions were made, but all of them are either specific to a single browser, or reliant on a third-party plugin.

Local Storage or DOM Storage or HTML5 storage, is a way for web pages to store named key/value pairs locally, within the client web browser, and will presist **even** when closing the web browser or navigating another web page.

## how to access and use

From your JavaScript code, you’ll access HTML5 Storage through the `localStorage` object on the global `window` object.

1. before using `localtorage` interface you have to check if the browser supports it.
2. you can access the object properties like any object in JavaScript.
    ex: `localStorage.setItem("bar", foo);`
3. to track changes on storage you can use event listeners associated with the window interface
    ex:

```javascript
                if (window.addEventListener) {
        window.addEventListener("storage", handle_storage, false);
        } else {
        window.attachEvent("onstorage", handle_storage);
        };
```  
