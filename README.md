# Install layoutmaterial 

1. **bower install** manviny/manviny.layoutmaterial --save  
2. check that all js and css libraries are loaded 
  index.html
  ```html
  <link rel="stylesheet" href="bower_components/manviny.layoutmaterial/layoutmaterial.css" />
  
  <script src="bower_components/angular/angular.js"></script>
  <script src="bower_components/angular-animate/angular-animate.js"></script>
  <script src="bower_components/angular-aria/angular-aria.js"></script>
  ```
3. **inject** ['ngMaterial', 'manviny.layoutmaterial'] into your app module  
4. **add** 'LoginCtrl','RegisterController' to your controller  
5. start using it  



# Example
```js
# app
angular.module('your-app', [..., 'ngMaterial','manviny.layoutmaterial', ...])
# controller
angular.controller('myCtrl', function ($scope, Login) {
    $scope.login = function(){
        Login.login({email:'usermail',password:'****'})
        .then(function(response){alert(JSON.stringify(response))})
```
