#jQuery UI Slider Pips (v1.3.0)  
###Plugin for adding little 'pips' and labels to a jQuery UI slider widget.      
  
  
This plugin **extends** the [jQuery UI Slider widget](http://jqueryui.com/slider/).    

Updated Documentation coming soon.

------------------------------------  
  
###Requirements:
  - jQuery (1.9+)
  - jQuery UI (1.10+)
  - A Reason to use it
  
------------------------------------  
  
###Usage:   
Include the plugin javascript file after jQuery & jQuery-ui.   
Include the CSS file; edit as you please.  
  
  
```javascript
// First of all attach a slider to an element.
$('.element')
  .slider({ opts });
```

```javascript
// Then you can give it pips and labels!  
$('.element')
  .slider({ opts })
  .slider('pips', {  
    first: 'label',  
    last: 'label',  
    rest: 'pip',  
    labels: ['label1', 'label2', ...],  
    prefix: "",  
    suffix: ""  
});
```

#####Options for pips:  
**first:** `'pip'` or `'label'` or `false`  
**last:** `'pip'` or `'label'` or `false`  
**rest:** `'pip'` or `'label'` or `false`  
**labels:** `['array','of','labels']` or `false`  
**prefix:** `"string"`  
**suffix:** `"string"`  


```javascript
// And finally can add floaty numbers (if desired)  
$('.element')
  .slider({ opts })
  .slider('pips', { opts })
  .slider('float', {  
    handle: true,  
    pips: true,  
    labels: ['label1', 'label2', ...],  
    prefix: "",  
    suffix: ""  
});
```

#####Options for float:  
**handle:** `true` or `false`  
**pips:** `true` or `false`  
**labels:** `['array','of','labels']` or `false`  
**prefix:** `"string"`  
**suffix:** `"string"` 


  
  
------------------------------------

###Style Customisation:  
All customisation should be done to the CSS file, or in your own CSS.  
The base styles I've provided do a decent job in the Demo,   
but they may need tweaking to suit your needs and UI theme.  
  
------------------------------------

###Compatibility:   
Modern Browsers, IE7+   
_(will need some CSS work for IE7 display issues, I'm not interested in doing them :P)_

------------------------------------

###License:  
Open Source MIT.  
http://opensource.org/licenses/MIT


------------------------------------

###Changlog:  

- **Mar 12, 2014** - Update to `1.3`
  - [Rewrite spacing and structure]()
  - [Add ability for custom labels on floats]()
  - [Fix bug of floats on labels >/< min/max in range]()

***

- **Nov 22, 2013** - CSS Changes
  - [Fix tiny bit of JS for vertical sliders](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/e7da19e5489c43ae2d439165199904812ee2e07f)
  - [Add missing CSS for vertical floats](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/d8ad4da1392f79f962b71aa842afee687d48ab57)

***

- **Aug 28, 2013** - Update to `1.2`
  - Convert to a grunt/node setup
  - Clean up code with jshint
  - Remove legacy demo

***

- **June 20, 2013** - Update to `1.1`
  - [Add ability to `prefix` and `suffix` labels and floats](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/cd483265a458ad1a3f200f16e4518a7f3d3db27a) - thanks [Xeeeveee](https://github.com/xeeeveee)
  - [Fix some bugs, clean up code](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/fda25f8545c941480fd10e6eb22e8efe91a78128)
  - update demo to show new features

***

- **March 13, 2013** - Update to `1.0`
  - [Add ability to create custom labels with an array](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/46467e05dd3c4ee0296b9a13cd9604a3ed8f2ff6#L2L9)
  - [Change `number` option to `label`](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/46467e05dd3c4ee0296b9a13cd9604a3ed8f2ff6#L2L9)
  - [Add `labels` option](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/46467e05dd3c4ee0296b9a13cd9604a3ed8f2ff6#L2L9)
  - [CSS style names changed to reflect update `ui-slider-pip-value`, `ui-slider-value` .. etc](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/46467e05dd3c4ee0296b9a13cd9604a3ed8f2ff6#L0L7)
  - fix various typos  
  
***

- **March 10, 2013** - Update to `0.2`
  - [Added extension for 'floating' numbers](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/aeacad87d47d79a96b9f26d2d83a5c3206d9f90f)
  - [Fixed so that sliders can start with negative numbers](https://github.com/simeydotme/jQuery-ui-Slider-Pips/commit/aeacad87d47d79a96b9f26d2d83a5c3206d9f90f)

------------------------------------  
