# Simple API KEYGEN

Generates a RFC4122 version 4 compliant UUID which can be used as an API Key. Semantics, heh.

The crypto.randomUUID() function is an emerging standard that is supported in Node.js and an increasing number of browsers.
```
function uuidv4() {
  return ([1e7]+-1e3+-4e3+-8e3+-1e11).replace(/[018]/g, c =>
    (c ^ crypto.getRandomValues(new Uint8Array(1))[0] & 15 >> c / 4).toString(16)
  );
}

console.log(uuidv4());
```

**Note: The use of any UUID generator that relies on Math.random() is strongly discouraged**

**Addition resources needed:**

**EXTERNAL JAVASCRIPT**
https//cdnjs.cloudflare.com/ajax/libs/jquery/2.1.3/jquery.min.js
