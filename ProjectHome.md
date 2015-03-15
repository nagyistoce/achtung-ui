# Achtung #
_achtung_ is a plugin for jQuery that creates notifications similar to those produced by [Growl](http://growl.info/).

Requires [jQuery](http://jquery.com/) 1.3.2.

This plugin utilizes portions of the CSS and icon framework from jQuery UI but does not require it.  The plugin operates independently to reduce dependencies.

## Demos ##

[Demos of v0.3.0](http://awgy.net/achtung/demo/)

![http://awgy.net/achtung/achtung-demos.jpg](http://awgy.net/achtung/achtung-demos.jpg)

## Example ##
```
// Create a new notification (5 second timeout)
$.achtung({message: 'Hello!', timeout:5});

// Create a new sticky notification, save as foo
foo = $.achtung({message: 'This will stay on-screen.', timeout: 0});

// Update with new message
foo.achtung('update', {message: 'Updated message!'});

// Close foo
foo.achtung('close');

// Remove all notifications
$('.achtung').achtung('close');
```