# jquery-handlebars-simple

Simple jQuery plugin to compile a template, process it with some data, and then
fill a DOM element with the results.

[Source](http://blog.teamtreehouse.com/handlebars-js-part-3-tips-and-tricks)

## Usage

```html
<html>
  <head>
    <script type="text/javascript" src="https://code.jquery.com/jquery-1.11.3.min.js"></script>
    <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/handlebars.js/4.0.5/handlebars.min.js"></script>
    <script type="text/javascript" src="https://cdn.rawgit.com/c-w/jquery-handlebars-simple/master/jquery-handlebars-simple.min.js"></script>

    <script type='text/javascript'>
      $(document).ready(function() {
        var data = { name: 'Alan' };
        $('#content').handlebars($('#template'), data);
      });
    </script>
  </head>

  <body>
    <script id='template' type='text/handlebars'>
      Hello, {{name}}
    </script>

    <div id='content'></div>
  </body>
</html>
```
