# Install layoutmaterial 

1. **bower install** manviny/manviny.layoutmaterial --save  
2. check that all js and css libraries are loaded  
3. **inject** 'manviny/manviny.layoutmaterial' into your app module  
4. **add** 'LoginCtrl','RegisterController' to your controller  
5. start using it  



# Needed
```js
# app
angular.module('your-app', [..., 'ngMaterial','manviny.layoutmaterial', ...])
# controller
angular.controller('myCtrl', function ($scope, Login) {
    $scope.login = function(){
        Login.login({email:'usermail',password:'****'})
        .then(function(response){alert(JSON.stringify(response))})
```
