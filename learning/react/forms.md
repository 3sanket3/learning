- If we want to passs parameters to to function on click we should use 

```javascript
onClick={
   this.functionToCall.bind(this,{param1 : 'value1',param2 : 'value2'})
} 

```
OR 

```javascript
onClick={() => {
    this.functionToCall({param1 : 'value1',param2 : 'value2'});
}} 

```