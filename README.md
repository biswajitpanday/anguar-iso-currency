# anguar-iso-currency
Ultimate Currency filter for country wise symbol and formatters

## How to Use : 

- Initialize Currency Filter to set some data in $rootScope :

```JavaScript
angular.module("ngApp", [...])
	.config(function($httpProvider, $stateProvider, $urlRouterProvider) {
		....
	})
	.controller('AppCtrl', function ($scope, $filter, $rootScope) {
		...
		$filter("isoCurrency")(0, 0, false);
	});
```

- Useage from inside Controller :

```JavaScript
return $filter("isoCurrency")(value, 2, false);
```
	
- Useage from inside Html :
```JavaScript
{{data.price | isoCurrency: 0 : false}}
```
