```ngmeta
name: PartIV Scope
completionMethod:
```
# Part IV… Scope

- Aapne scope pehle bhi padha hoga. **$scope** ke kaaran hum controller ke variables aur functions ko Html mei use kar pate hai. Jaise,

_app.js_

```javascript
angular.module(‘learn-scope’, []).controller(‘scope-ctrl’, [‘$scope’, function ($scope) {
	$scope.message1 = “This is a message stored in message1”;
}]);

```

_index.html_

```html
<p> {{ message1 }}</p>
```
- Magar, agar hum **var** ka use kar kar variable declare karenge tab uss variable ko hum Html mei use nhi kar payenge. Jaise neeche diya hua code galat hai,

_app.js_

```javascript
angular.module(‘learn-scope’, []).controller(‘scope-ctrl’, [‘$scope’, function ($scope) {
	var .message1 = “This is a message stored in message1”;
}]);
```
_index.html_

```html
<p> {{ message1 }}</p>
```

- Kyunki, **var** _Html aur Controller_ ko bind nhi karta magar **$scope** karta hai. 


