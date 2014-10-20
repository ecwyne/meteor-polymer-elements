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
  <!-- Add any <link rel="import" href="[path/to/element]"> tags you will use -->
	<link rel="import" href="bower_components/paper-checkbox/paper-checkbox.html">
</head>
<body>
  <!-- Simply use elements in body or in templates -->
	<paper-checkbox checked></paper-checkbox>
</body>
```
