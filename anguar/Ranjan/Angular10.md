```ngmeta
name: Scope Continued
completionMethod:
```
# Scope... Continued
- Abhi tak aapne jo bhi code kiya, usmei sirf **ek controller** banaya tha. Magar aisa ho sakta hai ki aapki app mei ek **se jyada controller** ho. Jaise, facebook website mei timeline ka ek controller ho sakta hai, notifications ka ek controller ho sakta hai.

- Aur jiss **Html tag** per aap controller define karte hai **wahan se** le kar uss tag ke **end tak** controller ka **scope** hota hai. Jaise,

_index html_

```html
<div ng-app = “learn-scope”>
    <div ng-controller = “counter” class = “first-div” > <!--counter scope-->
        <h1>{{ message }}</h1>
    </div>
    <div ng-controller = “stopWatch” class = “second-div”> <!--stopWatch scope-->
        <h1>{{ message }}</h1>                           
        <span>{{ message1 }}</span>
    </div> 
</div>
```

_apps.js_

```javascript
angular.module(‘learn-scope’,[])
     .controller(‘counter’,[‘$scope’, function ($scope) {
        $scope.message = ‘This message is from counter ctrlr’;
        $scope.message1 = “This variable is in counter scope”
    }]);

angular.module(‘learn-scope’)

    .controller(‘stopWatch’,[‘$scope’, function ($scope) {
        $scope.message = ‘This message is from stopwatch ctrlr’;
    }]);

```

- **first-div** ke h1 tag mei message ki value **counter controller** se aayegi. Aur **second-div** ke h1 tag mei **stopWatch controller** se.

- Magar second-div mei span tag mein **message1 ki value nhi aayegi** aur angular error throw karega kyunki message1 stopWatch ke **scope mein nahi** counter ke scope mei hai.

