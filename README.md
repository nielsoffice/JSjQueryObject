# JSjQueryObject Handling property and property method 
JavaScript jQuery Object 

```JS
 const jQueryObject = {
    
    name_id : {
    
      0 : 'id-1',
      1 : 'id-2'

    },
    result : function() {

      let pName = this.name_id;
        
      const FriendList = (function(z) {
  
        let newFriendName;
        let nnN = z;
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
            nnN,
            init,
            getNF,
        
        }

       })(pName);

       FriendList.init('firstName','lastName');

       return {
         getFullName : FriendList.getNF(),
         getObjectProperty : FriendList.nnN
       }
    
    }
 }

 jQueryObject.result();
 console.log(jQueryObject.result());

 // Object key base
 console.log(jQueryObject.result()['getFullName']);
```

```JS
// Result 
 {getFullName: 'firstName : lastName', getPropertyObject: {…}}
   getFullName : "firstName : lastName"
   getPropertyObject : {0: 'id-1', 1: 'id-2'}
  [[Prototype]] : 
  Object
 --------------------------------
   firstName : lastName
```

<br />Reference:
<br />https://github.com/nielsoffice/JSModulePattern
