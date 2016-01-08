# Install layoutmaterial ( roboto font, ngMaterial )

1. **bower install** manviny/manviny.layoutmaterial --save  
2. check that all js and css libraries are loaded and modules injected
  ###index.html
  ```html
  <link rel="stylesheet" href="bower_components/manviny.layoutmaterial/layoutmaterial.css" />
  
  <script src="bower_components/angular/angular.js"></script>
  <script src="bower_components/angular-animate/angular-animate.js"></script>
  <script src="bower_components/angular-aria/angular-aria.js"></script>
  <script src="bower_components/angular-material/angular-material.js"></script>
  <script src="bower_components/manviny.layoutmaterial/layoutmaterial.js"></script>
  ```
  ###app.js
  ```js
  
  # app
  angular.module('your-app', [..., 'ngMaterial','manviny.layoutmaterial', ...])
  
  # controller
  angular.controller('myCtrl', function ($scope, Login) {
    $scope.login = function(){
        Login.login({email:'usermail',password:'****'})
        .then(function(response){alert(JSON.stringify(response))})
  ```

3. start using it  



