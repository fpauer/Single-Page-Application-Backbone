# Single Page Application with Backbone 1.3.3

## Proposal

The idea is to check how is the entire process since install the js framework till the final version
of a simple SAP (Single Page Application).

## Some concepts about MVC (or derivatives, MVP / MVVM).

* A way of cleanly separating data, presenting data, and business logic (e.g. “To get the total exports of a country, you must sum its exports with every individual country”). Following definitions differ slightly depending on which interpretation you’re using, but the gist is similar.

	+ Model: Provider of data - could be an API. Could be a javascript object. Could be anything. It’s the “state” of the application, anything from the data in your viz to which buttons are current clicked and whether we’re showing exports or imports.
	+ Controller: Sits between everything and decides how to process the user input, where to gather data from, what to do with it, etc.
	+ View: e.g. templating - how the application actually looks to the user and where the user interacts with the application.

###Why? e.g.

* You can change the data source for a viz without changing any visualization code
* You can change the design of a viz to, say, use a different CSS library without changing UI logic
* Basically much less entanglement in general. http://programmers.stackexchange.com/questions/105352/why-should-i-use-an-mvc-pattern

###Some terminologies

* Two way data binding
	- I change something in the view (UI), the model (state data) changes automatically. I change the model, the view changes automatically. See: http://n12v.com/2-way-data-binding/ especially the angular example is pretty concise. Saves a lot of time and reduces bullshit boilerplate code.

* Dependency injection
	- A technique where the framework loads modules automatically for you. So let’s say your app needs a NetworkGraphVisualization and that one requires a D3Visualization and a SliderWidget, which in turn requires JQuery, a dependency injection framework will initialize all that junk for you. This also encourages separation of concerns.

		+ Routing: Being able to index a specific view in the app with a specific URL and having the URL change with the app state.
		+ Templates: You define the structure of HTML and provide slots, then you can plug in any data you want. Can be generated from a string with templating code in it or by writing html-like DOM stuff - handlebars is the former and Angular directives is the latter.


## Pre-requisities - http://backbonejs.org

Backbone's only hard dependency is Underscore.js. 
For RESTful persistence and DOM manipulation with Backbone.View, include jQuery ( >= 1.11.0), and json2.js for older Internet Explorer support. 


## Installation


## Pros
- Who comes from a Jquery background , backbone provides a good integration with Jquery ( >= 1.11.0). 

## Cons


## Conclusion
