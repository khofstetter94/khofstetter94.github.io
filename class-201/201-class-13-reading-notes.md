# Local Storage

- [The Past, Present, and Future of Local Storage for Web Applications](http://diveinto.html5doctor.com/storage.html)

- If your native client application needs local storage beyond key/value pairs, you can embed your own database, invent your own file format, or any number of other solutions

- **Downsides of cookies**: they are included with every HTTP request therefore they slow down your web app by transmitting the same data over and over and also this sends data unencrypted over the internet. Also, they are limited to about 4KB of data

- **What we want** - a lot of storage space, on the client, that persists beyond a page refresh, and isn’t transmitted to the server

## Brief History of Local Storage Hacks before HTML

- **userData** - allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure

- **Flash** gives each domain 100 KB of storage “for free”, Beyond that, it prompts the user for each order of magnitude increase in data storage (1 Mb, 10 Mb, and so on)

- **Gears** - After obtaining permission from the user once, Gears can store unlimited amounts of data per domain in SQL database tables

## HTML5 Storage

- **HTML5** - a way for web pages to store named key/value pairs locally, within the client web browser. Supported by the latest version of pretty much browser. From your JavaScript code, you’ll access HTML5 Storage through the localStorage object on the global window object.

- If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.

- **setItem()** - with a named key that already exists will silently overwrite the previous value

- **removeItem() and void clear()** - removing the value for a given named key, and clearing the entire storage area

- property to get the total number of values in the storage area, and to iterate through all of the keys by index (to get the name of each key):

        interface Storage {
          readonly attribute unsigned long length;
          getter DOMString key(in unsigned long index);
        };

- **Storage Event** - keep track of when the storage area changes by trapping the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something

- **Limitations of HTML5 Storage** - “5 megabytes" - how much storage space each origin gets by default, “QUOTA_EXCEEDED_ERR" - the exception that will get thrown if you exceed your storage quota of 5 megabytes, and “no" - the answer to the next obvious question, “Can I ask the user for more storage space?”

- with HTML5 Storage, we can save the progress locally, within the browser itself

- The Indexed Database API exposes what’s called an object store. An object store shares many concepts with a SQL database. The primary difference is that the object store has no structured query language.

[Return home](https://khofstetter94.github.io/reading-notes/)
