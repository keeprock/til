I'm always struggle with simple basic setup for angular js 1.

Here you go - stop worrying and start doing it.

```html
<!DOCTYPE html>
<html lang="en" ng-app="app">
<head>
    <meta charset="UTF-8">
    <title>File manager</title>

    <script src="https://cdnjs.cloudflare.com/ajax/libs/angular.js/1.6.5/angular.min.js"></script>
    <script src="./src/bundle.js"></script>
</head>
<body>

<div>
    <div ng-controller="MyController as ctrl">
        {{ctrl.test}}
    </div>
</div>

</body>
</html>
```

```js
let app = angular.module('app', []);

app.controller('MyController', ['$scope', function($scope) {
        let ctrl = this;
        ctrl.test = 'hi!';
}]);
```