# Obtener-la-moda-de-un-numero-en-javascript

```javascript
function findMode(a){
    var index = 0;
    var soFar = 1; 
    var count = 1; 
    for(var k =1; k < a.length; k++){
        if (a[k-1] == a[k]){
            count++;
        }
        if(count > soFar){ 
            soFar = count; 
            index = k; 
        }
        else {
            count = 1; 
        }
    }
    return a[index]; 
}
```
