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
