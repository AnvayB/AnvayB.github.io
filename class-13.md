# Local Storage
- HTML5 storage is web storage
  - aka DOM storage
- way for web pages to store named key/value pairs locally
  - in the client's web browser (like cookies)
- data persists after you navigate away from that web page, close the tab, or exit the browser
- unlike cookies, the data isn't sent to a remote web server
- it is implemented natively in web browsers
- check for HTML5 storage
```js
function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}
```
- using HTML5 storage
  - data being stored can be of any type: string, Boolean, number, etc
  - data actually stored as a string
