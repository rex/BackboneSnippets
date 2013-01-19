Backbone Snippets
===

Yo. What's up? Oh, yeah, you're here for the awesometastic Sublime Text 2 snippets for Backbone.js. Right this way!

Tab Completion Snippets
---

> Remember! Put these in your `Packages\User` directory, wherever that is. On Windows 8, it's located at `C:\Users\Pierce\AppData\Roaming\Sublime Text 2\Packages\User`.

Short Text | Object Created  
-----------|--------------  
`bbcoll` | new `Backbone.Collection`  
`bbmodel` | new `Backbone.Model`  
`bbview` | new `Backbone.View`  

Full Tab Completion Output
---

`bbcoll`
---

Type `bbcoll`, press `tab`, and you get this:

	Application.Collection =  Backbone.Collection.extend({
		model : 'ModelName',
		initialize : function() {
			// Initialization
		},
		render : function() {
			// Do stuff!
		}
	});

`bbmodel`
---

Type `bbmodel`, press `tab`, and you get this:

	Application.Model =  Backbone.Model.extend({
		idAttribute : '_id',
		initialize : function() {
			// Initialization
		}
	});

`bbview`
---

Type `bbview`, press `tab`, and you get this:

	Application.View =  Backbone.View.extend({
		el : 'Parent',
		tagName : 'TagName',
		className: 'ClassName',
		events : {
			// All event delegators here
		},
		initialize : function() {
			// Initialization
		},
		render : function() {
			// Put the thing on the page!
		}
	});

Enjoy! Shoot me an email if you have any questions or additions, and remember that pull requests are always welcome!

Pierce 

[@kiapierce](http://www.twitter.com/kiapierce)  
`pierce@piercemoore.com`  
[PierceMoore.com](www.piercemoore.com)
