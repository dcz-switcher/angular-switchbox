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
2 - add the module to your application module
```
<script>
(function () {
    var MyApplication = angular.module('MyApplication', ['mx']);
}());
</script>
```
3 - use it in html
```
<div mx-switchbox></div>
```
3.1 - you can bind the switchox state to a model
```
// for example you have a model like that :
myModel = {
booleanData : true;
};

// you can now bind with switched attribute :
<div mx-switchbox switched="myModel.booleanData"></div>
```
