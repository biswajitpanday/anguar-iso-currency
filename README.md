# anguar-iso-currency
Ultimate Currency filter for country wise symbol and formatters

## How to Use : 

- Initialize Currency Filter to set some data in $rootScope :
	angular.module("ngApp", [...])
		.config(function($httpProvider, $stateProvider, $urlRouterProvider) {
			....
		})
		.controller('AppCtrl', function ($scope, $filter, $rootScope) {
			...
			$filter("isoCurrency")(0, 0, false);
		});

- Useage from inside Controller :
	return $filter("isoCurrency")(value, 2, false);
	
- Useage from inside Html :
	{{data.price | isoCurrency: 0 : false}}