
Simple-button-checks 3
==========
Transform checkbox inputs to Bootstrap HTML buttons

## Demos / Documentation
Demo and doc : [http://joelthorner.github.io/simple-button-checks/](http://joelthorner.github.io/simple-button-checks/)

## Getting Started

### Includes
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <link rel="stylesheet" href="path/to/simple-button-checks.css">
  </head>
  <body>

    <script src="path/to/jquery/3.x.x.min.js"></script>
    <script src="path/to/simple-button-checks.js"></script>
  </body>
</html>
```

### Js initialization
```javascript
//default options
$('input[type="checkbox"]').simpleButtonChecks({
  buttonClass: "sbc-default",
  checkedIcon : '<svg aria-hidden="true" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512"><path d="M173.898 439.404l-166.4-166.4c-9.997-9.997-9.997-26.206 0-36.204l36.203-36.204c9.997-9.998 26.207-9.998 36.204 0L192 312.69 432.095 72.596c9.997-9.997 26.207-9.997 36.204 0l36.203 36.204c9.997 9.997 9.997 26.206 0 36.204l-294.4 294.401c-9.998 9.997-26.207 9.997-36.204-.001z"/></svg>',
  nonCheckedIcon : '',
  // 'none' or 'input' or 'all'
  wrapContainer : 'none', 
  // add click listener if label has rel with label for -> input id
  // <label for="country"></label> <input id="country" type="checkbox">
  strictLabel : true,
  btnAttributes : {
    'type' : 'button'
  },
  onInit : null,
  onChange : null,
  changeCallback : null,
  onDestroy: null
});

//equivalent of
$('input[type="checkbox"]').simpleButtonChecks();
```

## Options and Methods
Options and Methods : [http://joelthorner.github.io/simple-button-checks/](http://joelthorner.github.io/simple-button-checks/)

## Changelog
- Removed bootstrap option
- Removed size option
- BtnClass option named to buttonClass
- Renamed namespaces 'sbtc' to 'sbc'
- Basic CSS It is better to customize it according to the project
- Check icon to innerHTML svg
- Renamed plugin
- New documentation
- New id for buttons created