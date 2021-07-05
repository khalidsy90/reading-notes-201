# LocalStorage

* In simple terms, the **local storage** can be compared to a data base, except it's found in a browser and not on a server. It's basically a huge Javascript object inside which we are able to store data in the form of key-value pairs.
* The data you store in the localStorage never leaves you machine

> the localStorage read-only property of the window interface allows you to access a Storage object for the Document's origin;
the stored data is saved across browser sessions.

The way we can access this ```storage``` object and populate the two columns is by making use of some specific methods.

local storage is read-only, meaning we can add, read and delete data from it but we can't modify it (at most, we can overwrite the previous value of a key, by re-adding to the storage, using the same key and the new value we want to store).

For access we should use the following syntax:

```javascript
window.localStorage 
//or 
localStorage
```

If we want to add something, we can do it like this:

```javascript
localStorage.setItem("key", "value");
```

To access a value, we write this:

```javscript
localStorage.getItem("key");
```

And lastly, we can delete one specific value:

```javascript
localStorage.removeItem("key");
```

Or we can clear the whole local storage:

```javascript
localStorage.clear();
```

> One important thing to remember is that the localStorage can store only strings. To store objects, we must first convert them to strings using the JSON. ```stringify()``` method. And we convert the strings back into objects, after we retrieve them from the localStorage, using the ```JSON.parse()```.

* We can add as many key-value pairs as we want as long as the data doesn't exceed 5MB.
  
### THINGS TO REMEMBER ABOUT THE LOCAL STORAGE

**- it is tab specific, meaning each browser tab we open will have different data in the localStorage(this doesn't apply if the tabs have the same origin (share the same domain))**

**- some browsers, when used in incognito mode don't allow for setting data in the localStorage it is synchronous, meaning each operation will execute one after the other (this might work for small projects, but it will impact the runtime of the more complex ones)**

**- it can only store data string data (this is fine for small projects, but it can be cumbersome to serialize data in complex ones)**

### SUPER IMPORTANT THING TO REMEMBER

**- Local storage should under no circumstances be used to store sensitive information (e.g. passwords or personal details), since the data inside it can be accessed from anywhere on the page (it has no real protection and it's susceptible to cross-site scripting).**  