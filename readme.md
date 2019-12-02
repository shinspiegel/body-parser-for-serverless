This is a simple parser for body form on multipart form, similar to multer, but this is a simple, yet usefull parser.

I did not create all this code, some of the code I did used from other sources, I just created a simples promise object for ease to use. I guess other should have created it before me.

## Why I did this?

I was looking for a body parser for images, this is the principal use of this parser.
I guess it could work for any file, but the main reason was images.

## How to use?

Just pass the event object to the parser function and it will return the body parts of the files and objects.

### Exemple

```js
"use strict";

module.exports.v1 = async (event, context) => {
  //this is the parsed body.
  const parsedBody = await Parser(event);

  return {
    statusCode: 200,
    body: "Working"
  };
};
```

If you like it, please give a star.
