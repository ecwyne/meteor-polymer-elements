#Meteor-Polymer

Add the magic of web components and [Polymer](http://polymer-project.org) to [Meteor](http://meteor.com)!

##About
This package adds [core-elements and paper-elements](http://www.polymer-project.org/docs/elements/) from Polymer.

##How to Install

```bash
meteor add ecwyne:polymer-elements
```

##How to Use
Simply follow the instructions layed out on [polymer-project.org](http://www.polymer-project.org/docs/start/usingelements.html). Step 1 is already taken care of for you!

After your first `meteor run` you can browse your `[APP_DIR]/public/bower_components/` directory to find installed elements. See below for how to `<link rel="import"` these elements and start using them!

###Example
```html
<head>
	<link rel="import" href="bower_components/core-ajax/core-ajax.html">
</head>
<body>
	<core-ajax url="//example.com/json" handleAs="json"></core-ajax>
	<script>
      // Wait for 'polymer-ready'. Ensures the element is upgraded.
      window.addEventListener('polymer-ready', function(e) {
        var ajax = document.querySelector('core-ajax');

        // Respond to events it fires.
        ajax.addEventListener('core-response', function(e) {
          console.log(this.response);
        });

        ajax.go(); // Call its API methods.
      });
    </script>
</body>
```
