![DroneDeploy](http://www.getprowl.com/images/dd.png)

 
### DroneDeploy: PDF tile images retrieved via Tiles


## How it works

How I've improved it is with using less resources (for faster load times, and using it on older machines) which you can view within the source code, I still ended up using pdfmake, although there are better tools like wkhtmltopdf, and Prawn (which is Ruby based) and the Tiles API, decided to Deploy via Herokuish, Herokuish uses PHP

https://github.com/gliderlabs/herokuish

## Express.js

For obvious reasons, just proxying requests, via using CORS is not as simple as specifying the appropriate server URL. There are a lot of changes necessary on both the server and client tiers to get it working. It ismuch simpler to proxy your HTTP requests via a server running on your domain, also as usual used JS Promises. Promises will handle any exceptions (both explicit and implicit) in asynchronous code blocks that use then(). I was considering using "bluebird", using ```Promise.promisifyAll```, an example of using bluebird, would be something similar to this, in this type of scenario:

```javascript
Promise.promisifyAll(
    Object target,
    [Object {
        suffix: String="Async",
        multiArgs: boolean=false,
        filter: boolean function(String name, function func, Object target, boolean passesDefaultFilter),
        promisifier: function(function originalFunction, function defaultPromisifier)
    } options]
) -> Object
```
https://github.com/expressjs/express

https://github.com/petkaantonov/bluebird

## Sass 

Used Sass and a few mixins to use less resources, under 100 lines of code

https://github.com/sass/sass

