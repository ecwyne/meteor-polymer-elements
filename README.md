# Meteor-Polymer

Add the magic of web components and [Polymer](http://polymer-project.org) [(0.5.5)](https://github.com/polymer/polymer/releases) to [Meteor](http://meteor.com)!

## About
This package adds [core-elements and paper-elements](http://www.polymer-project.org/docs/elements/) from Polymer.

##How to Install

```bash
meteor add ecwyne:polymer-elements
```

## How to Use
All necessary web components and routing is done for you! All you have to do is use them! See below for how to import these elements and start [using them](https://www.polymer-project.org/0.5/docs/start/usingelements.html#using)! 

## Examples
Check out the [wiki](https://github.com/ecwyne/meteor-polymer-elements/wiki/Examples)!
###### automatic_helper.html
```html
  <!-- replace dashes with underscores for any element -->
	{{> paper_checkbox attrs=attributeObject}}
```
##### automatic_helper.js
```js
  Template.automatic_helper.helpers({
    attributeObject = function(){return {checked: true}}
  })
```
###### link_helper.html
```html
  <!--use a helper to import the link tags automatically -->
    {{> paper_checkbox_link}}
  <!-- Use the component as you normally would -->
	<paper-checkbox checked></paper-checkbox>
```
###### vanilla_polymer.html
```html
  <!-- Add any <link rel="import" href="[path/to/element]"> tags you will use -->
	<link rel="import" href="bower_components/paper-checkbox/paper-checkbox.html">
  <!-- Use the component as you normally would -->
	<paper-checkbox checked></paper-checkbox>
```
##### block_helper.html
```html
  {{#paper_button}}Submit!{{/paper_button}}
```
