### .delete\(ID\) {#delete}

> **Input:                        
>    **ID -&gt; String
>
> **Returns: **Promise&lt;boolean&gt; _\(If successfully deleted\)_

```js
let data = { username: 'TrueXPixels', balance: 100 };
db.set('uniqueID', data).then(i => {
    console.log(typeof i) // 'object'
    console.log(i); // { username: 'TrueXPixels', balance: 100 }
    console.log(i.username); // 'TrueXPixels'
})

db.delete('uniqueID').then(i => console.log(i)); // True
db.fetch('uniqueID').then(i => console.log(i)); // null
```

---



