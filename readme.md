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

	Module.SubModule = Backbone.Collection.extend({
		model : ModelName,
		initialize : function() {
			console.log("Initializing  Collection");
			// Initialization
		}
	});

`bbmodel`
---

Type `bbmodel`, press `tab`, and you get this:

	Module.SubModule = Backbone.Model.extend({
		idAttribute : '_id',
		defaults : {
			//
		},
		initialize : function() {
			console.log("Initializing  Model");
			// Initialization
		}
	});

`bbview`
---

Type `bbview`, press `tab`, and you get this:

	Module.SubModule = Backbone.View.extend({
		el : 'Parent',
		tagName : 'TagName',
		className: 'ClassName',
		dispatcher : _.clone(Backbone.Events),
		template : _.template(  ),
		events : {
			// All event delegators here
		},
		initialize : function() {
			console.log("Initializing  View");
			this.listenTo(this.model, "change", this.render);
		},
		render : function() {
			// Put the thing on the page!
			var self = this;

			return this;
		}
	});

Enjoy! Shoot me an email if you have any questions or additions, and remember that pull requests are always welcome!

Pierce 

[@kiapierce](http://www.twitter.com/kiapierce)  
`pierce@piercemoore.com`  
[PierceMoore.com](www.piercemoore.com)
