angular-switchbox
=================

An autonome directive that show a switchbox over an input checkbox tag

For my needs, I have to support ie8, so I choose the simpliest way and use a base64 image for the switchbox

I think developping a Polymer version soon

result :

![](https://github.com/dcz-switcher/angular-switchbox/blob/master/switchbox.svg)


how to use :

1 - load js in your html :
```
<script src="js/mx/mxSwitchbox.js"></script>
```
2 - add the 'mx' module to your application module
```
<script>
(function () {
    var myApplication = angular.module('MyApplication', ['mx']);
}());
</script>
```
3 - use it in html
```
// for example you want to bind to the boolean value isShiny in your controller :
myApplication.controller('MyController', [function () {
this.isShiny = true;
}]);

// you can bind with switched attribute :
<div ng-controller="MyController as myCtrl">
<div mx-switchbox switched="myCtrl.isShiny"></div>
</div>
```
