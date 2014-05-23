#docs/core/README.md
==============

The core documentation.
![Image](../core/images/system_overview_core.png?raw=true)

##About core
Core is the **business** layer.

##Architecture
The architecture is service oriented.
![Image](../core/images/architecture_overview_core.png?raw=true)

##View
The view knows only about itself and its viewService.

##ViewController
The viewController knows about itself, its view(s) and their viewService(s).

##ViewService
The viewService know only about the serviceBus.

##ServiceBus
The serviceBus knows only about itself.

##ServiceModel
The serviceModel knows about itself, the serviceBus and its model(s).

##Model
The model knows only about itself.

##Modules are following the Asynchronous Module Definition (AMD) pattern
See https://www.youtube.com/watch?v=HwO_qwcJ4rs

For example:
```
/*
* Main
*
* Depends on: add, subtract, square, divide
*/
require(
	{ 
		paths:	{}
	},
	['add','subtract','square','divide'],
	function(add, subtract, square, divide) {
		console.log(add(6,1));
		console.log(subtract(6,1));
		console.log(square(4));
		console.log(divide(16,4));
	}
);

/**
* Multiply
*
* Depends on: none
*/
define(function(){
	return function(x,y){
		return x * y;
	};
});

/**
* Square
*
* Depends on: multiply
*/
define(['multiply'], function(multiply){
	return function(x){
		return multiply(x,x);
	};
});
```
