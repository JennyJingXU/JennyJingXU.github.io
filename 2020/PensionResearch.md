# Download All Files for Form 5500 by Mocking Click in Chrome Console

## get the link of all corresponding links ending with `.zip`
Output is [*NodeList*](https://developer.mozilla.org/en-US/docs/Web/API/NodeList), with few operation options
```
var linkList = document.querySelectorAll('a[href$=".zip"]');
```
## initiate an array
```
var linkArray = new Array();
```
## add the elements in the NodeList to the array
```
for (var i =0; i<linkList.length; i++){
 linkArray.push(linkList[i]); 
}
```
## click the elements every 1000 ms, by getting and deleting the first item in the array
```
setInterval(function () {
    var here = linkArray[0];
    linkArray.shift();  
    here.click(); 
		},1000)
```
