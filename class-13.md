# Local Storage

## The Past, Present, and Future of Local Storage for Web Applications

Very early throughout the web’s history cookies have existed and were used for persistent local storage of small amounts of data. However, cookies have three disadvantages. First, they slow down your web application, due to the fact that they transmit the same data over and over again. Secondly, they send data over the web unencrypted, and third they are limited to 4 KB of data, which is enough to slow down your application, but not enough to be beneficial to the user. Nowadays, most users would like to have a lot of storage space, on the client, that persists beyond a page refresh, and isn’t transmitted to the server. This was not achievable until HTML5.

Microsoft’s came up with DHTML Behaviors, and one of those behaviors was called userData, which was built into their Internet Explorer web browser. userData enabled web pages to store up to 64 KB of data per domain. In 2002 Adobe introduced Local Shared Objects, which enabled flash objects to store up to 100 KB of data per domain. Gears was launched by Google in 2007. Gears was an open source browser plugin with the intent of providing additional capabilities in the browsers. Gears enables the browser to store unlimited amounts of data per domain in SQL database tables. Eventually HTML5 would solve this problem of different storage limitations, by providing a standard API, which was implemented natively and consistently in multiple browsers, without having to rely on third party plugins. 

HTML5 storage is a way for web pages to store named key/value pairs locally, within the client web browser. From your JavaScript code, you’ll be able to access HTML5 storage through the localStorage object on the global window object; however, you should verify whether the browser supports it. In order to do so, you can check for HTML5 storage by……

function supports_html5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] !== null;
  } catch (e) {
    return false;
  }
}


You can also use the Modernizr to detect support for HTML5 storage.


if (Modernizr.localstorage) {
  // window.localStorage is available!
} else {
  // no native support for HTML5 storage :(
  // maybe try dojox.storage or a third-party solution
}

*(Pilgrim, Mark, “The past, present & future of local storage for web applications”, 2009-2011)*



When you are using HTML5 storage, it’s important to know that it is based on named key/value pairs. Data is stored by you, and it is based on a named key. Whenever you retrieve that data, you use the same key. The named key is a string. The data can be any type supported Javascript, which includes booleans, integers or floats, but when the data is stored, it’s stored as a string. In the event that you are storing and retrieving anything other than a string, then you will have to use functions such as parseInt( ) or parseFloat( ) , in order to make your retrieved data into one of the JavaScript data type. *(Pilgrim, Mark, “The past, present & future of local storage for web applications”, 2009-2011)*