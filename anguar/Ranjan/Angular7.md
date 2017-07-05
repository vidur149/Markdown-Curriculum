```ngmeta
name: Counter Continued
completionMethod:
```
# Counter... Continued
- Controller mei hum **variables** aur **functions** define kar sakte hai. Inn variables aur functions ko Html mei use karne ke liye **$scope** ka use kiya jaata hai. $scope humein apne controller mei inject karna hota hai yaani ki controller mei daalna hota taaki hum usse use kar paaye.
```javascript
angular.module(‘app ka naam’, [])
	.controller(‘controller ka naam’, [‘$scope’, function($scope) {
	   	// controller logic
	}]);
```
- Jaise hum Jquery mei click event par function call karte hai, ussi tarah hum html tag par 
    ```<html_tag ng-click = “function ka naam”>``` se controller ka function **click** par call kar sakte hai. 

   **Assignment karne se pehle, yeh concepts padho aur samjho:**
    	- **Data-Binding**, [en](http://learnkode.com/Tutorial/Angular/angular-databinding), hi
    	- **Angular-controller** [en](https://www.w3schools.com/angular/angular_modules.asp#ez-insert-after-placeholder-124), hi
	    - **ng-click** [en](http://tutlane.com/tutorial/angularjs/angularjs-ng-click-event-function-with-example), hi
	    - **Scope**, [en](https://www.w3schools.com/angular/angular_scopes.asp), hi


        
