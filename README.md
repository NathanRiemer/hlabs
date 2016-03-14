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

`div {background:#fff;}` -- **applies to div elements**

`#div {background:#fff;}` -- **applies to the element with the id 'div'**

`.div {background:#fff;}` -- **applies to elements with the class 'div'**

## 7. What is the difference between these 2 uses of the `<script>` tag?

`<script src=”http://example.com/whatever.js”></script>` -- **goes to the url and runs the code there**

`<script>var whatever = true</script>` -- **runs the javascript within the script tags, in this case assigning the variable 'whatever' the value true.**

## 8. What is the difference between these two javascript snippets?

`var x = function() {
  return 1+1;
}();` -- **x is 2.**

`var y = function() {
  return 1+1;
};` -- **x is a function that when invoked will return 2.**

# Developer Quiz Practical

## 1. [Solution](practical1.html)

## 2. Tracking Pixel

### a. 

Caching is a problem because if a client has cached the pixel they will not need to request it from our site after their initial visit, and thus we will not be able to include subsequent visits in our visitor total.

### b. 

To prevent browser caching of the pixel image I could append a randomized query string to the image url so that each time the page is visited the client browser perceives it as a new image to be downloaded.

### c. 

If the website is served over HTTPS and the pixel is as specified above the browser will raise a warning about unsecure content. We could fix this by updating the tracking pixel's url to a relative url, so that it will use https when appropriate. 

*I had to look this one up, I used information I found [here](https://productforums.google.com/forum/#!topic/tag-manager/gr8q46Fpy5c)*

### d. 

The tracking company could collect all the information included in the HTTP request, which includes IP address and hostname, the browser type, and the language.

### e.

I believe a script tag might allow more information about the client to be collected, such as plugin support.


