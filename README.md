# JSjQueryObject
JavaScript jQuery Object 

```JS
 const jQueryObject = {
    
    name : "myName",
    result : (function() {
  
        let newFriendName;
        let name;
        let lastName;
        
        // Custom constructor or setter !
        const init = function(x, y) {
            name = x;
            lastName = y;
        }
        
        const getNF = function() { 
            return name +' : '+lastName; 
        }

        // Expose public data 
        return {
            init,
            getNF
        }

    })()

 }

 jQueryObject.result.init('myName','LastName');
 console.log(jQueryObject.result.getNF());
 
```

<br />Reference:
<br />https://github.com/nielsoffice/JSModulePattern
