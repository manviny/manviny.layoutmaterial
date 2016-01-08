# Install layoutmaterial ( Roboto fonts, ngMaterial )

1. **bower install** manviny/manviny.layoutmaterial --save  
2. check that all js and css libraries are loaded and modules injected

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
  
  ###index.html
  ```html
  <meta name="viewport" content="initial-scale=1, maximun-scale=1, user-scalable=no">

  <link rel="stylesheet" href="bower_components/manviny.layoutmaterial/layoutmaterial.css" />
  <link href='https://fonts.googleapis.com/css?family=Roboto:400,500,700,400italic' rel='stylesheet' type='text/css'>
  
  <style>
 /* if you want to include roboto manually */
    @font-face {
      font-family: 'MyFontFamily';
      src: url('../robotomono-googlefont/RobotoMono-Medium.ttf')  format('truetype'),
      src: url('../robotomono-googlefont/RobotoMono-Regular.ttf')  format('truetype');
    }   
  </style>


  <script src="bower_components/angular/angular.js"></script>
  <script src="bower_components/angular-animate/angular-animate.js"></script>
  <script src="bower_components/angular-aria/angular-aria.js"></script>
  <script src="bower_components/angular-material/angular-material.js"></script>
  <script src="bower_components/manviny.layoutmaterial/layoutmaterial.js"></script>
  ```


3. start using it  



