**How to use**

In Cloud Code:

```javascript
var parseFindAll = require('cloud/parseFindAll.js');
var myQuery = new Parse.Query("Whatever");
myQuery.equalsTo("foo","bar");
parseFindAll(myQuery).then(function(results){
	
	console.log(results.length);
	// results contains the WHOLE data of the table
});
```

Browser side:

You need to include async.js first; parseFindAll function will be available on the window scope
