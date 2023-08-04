
# dummy-website
This website was created to test little things

 - Page visibility
 - Something else

---

## Page Visibility API

The Page Visibility API is built into modern web browsers and is accessible through JavaScript. It provides a standardised way to determine the visibility state of a web page and to receive notifications when the visibility state changes.

The API is supported by most modern web browsers, including Chrome, Firefox, Safari, Edge, and others. This means that you can use the Page Visibility API in your web applications without needing to install any additional libraries or frameworks.

### How to Use

1. Access the visibility state using the `document.visibilityState` property. This property provides a string that indicates whether the page is "visible," "hidden," "prerender," or "unloaded."

2. Listen for the `visibilitychange` event on the `document` object. This event is fired whenever the visibility state of the page changes.

3. In the event handler for the `visibilitychange` event, you can check the value of `document.visibilityState` to determine the current visibility state of the page. Based on the state, you can take appropriate actions.

Here's the basic JavaScript code snippet:

```javascript
function handleVisibilityChange() {
    if (document.visibilityState === 'visible') {
        console.log('User returned to the tab');
    } else if (document.visibilityState === 'hidden') {
        console.log('User left the tab');
    }
}

// Add an event listener to the visibilitychange event
document.addEventListener('visibilitychange', handleVisibilityChange);
```

## How to test

To test the Page Visibility API function, you can follow these steps:

1. Open index HTML file in a web browser.

3. Open the browser's developer console. You should see console log messages indicating whether the user has returned to or left the tab as you switch between the browser tab and other applications.
