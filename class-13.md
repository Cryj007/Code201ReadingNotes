# “The Past, Present, and Future of Local Storage for Web Applications”

###Notes
- Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
- Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
- Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful
- userData allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure.
- HTML5 Storage is a way for web pages to store named key/value pairs locally, within the client web browser.
 
 #####HTML 5
- based on named key/value pairs.
- store data based on a named key to be able to retrieve that data with the same key
- The named key is a string.
- data is actually stored as a string

- Calling setItem() with a named key that already exists will silently overwrite the previous value.
- Calling getItem() with a non-existent key will return null rather than throw an exception.
- The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something.
- “5 megabytes” is how much storage space each origin gets by default.
- “QUOTA_EXCEEDED_ERR” is the exception that will get thrown if you exceed your storage quota of 5 megabytes.
- Data is stored as strings. If you are storing something other than a string, you’ll need to coerce it yourself when you retrieve it. 

  #####Object Store
- shares many concepts with a SQL database
- There are “databases” with “records,” and each record has a set number of “fields.”
- Each field has a specific datatype, which is defined when the database is created.
- can select a subset of records, then enumerate them with a “cursor."
- Changes to the object store are handled within “transactions.”



### Vocab
- KEY= string; the named key that was added, removed, or modified

- OLDVALUE= any; the previous value (now overwritten), or null if a new item was added

- NEWVALUE= any; the new value, or null if an item was removed

- URL= string; the page which called a method that triggered this change
