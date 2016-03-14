# Developer Quiz Questions

## 1. What is the difference between HTTP and HTTPS?

HTTPS is an encrypted form of HTTP. It allows for more secure communication between clients and servers.

## 2. What is the difference between HTTP GET and POST?

A POST request has a body that contains data, while a GET request does not. POST requests are often used for form submission.

## 3. What is the difference between the HTTP 2xx status codes and 4xx status codes?

HTTP 2xx codes indicate success while 4xx codes indicate an error has occurred (and is attributed to the client, as differentiated from HTTP 500 which indicates the error is on the server side).

## 4. What is ajax (conceptually, what does it do)? Describe a situation where it is useful.

AJAX allows a client to query and receive data from a server without refreshing the whole webpage. One situation where it might be used is to provide search predictions as a user is typing their query into a search bar.

## 5. What is responsive design?

Websites built with responsive design will adapt appropriately to various display sizes.

## 6. What is the difference between these 3 CSS rules?

`div {background:#fff;}` -- applies to div elements.

`#div {background:#fff;}` -- applies to the element with the id 'div'

`.div {background:#fff;}` -- applies to elements with the class 'div'

## 7. What is the difference between these 2 uses of the <script> tag?

`<script src=”http://example.com/whatever.js”></script>` -- goes to the url and runs the code there

`<script>var whatever = true</script>` -- runs the javascript within the script tags, in this case assigning the variable 'whatever' the value true.

## 8. What is the difference between these two javascript snippets?

`var x = function() {
  return 1+1;
}();` -- x is 2.

`var y = function() {
  return 1+1;
};` -- x is a function that when invoked will return 2. 

# Developer Quiz Practical

## 1. [Solution](practical1.html)