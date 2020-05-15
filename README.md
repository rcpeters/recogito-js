<p align="center">
  <br/>
  <img width="310" src="https://raw.githubusercontent.com/recogito/recogito-js/master/recogitojs-logo-white-small.png" />
  <br/><br/>
</p>

A JavaScript library for text annotation. Use it to add annotation functionality to a web page, or as a toolbox 
for building your own, completely custom annotation apps. Try the [online demo](https://recogito.github.io/recogito-js/)
or see the [API reference](https://github.com/recogito/recogito-js/wiki/API-Reference).

![Screenshot](screenshot.png)

## Resources

- [Introduction](https://github.com/recogito/recogito-js/wiki)
- [API Reference](https://github.com/recogito/recogito-js/wiki/API-Reference)
- [Demo](https://recogito.github.io/recogito-js/)

## Installing

If you use npm, `npm install @recogito/recogito-js`. Otherwise download the 
[latest release](https://github.com/recogito/recogito-js/releases/latest).

```html
<script src="recogito.min.js"></script>
```

## Using

```html
<body>
  <pre id="my-content">My text to annotate.</pre>
  <script type="text/javascript">
    (function() {
      var r = Recogito.init({
        content: document.getElementById('my-content')
      });

      // Add an event handler  
      r.on('createAnnotation', function(annotation) { /** **/ });
    })();
  </script>
</body>
```

Full documentation is [on the Wiki](https://github.com/recogito/recogito-js/wiki). Questions? Feedack? Feature requests? Join the 
[RecogitoJS chat on Gitter](https://gitter.im/recogito/recogito-js).

[![Join the chat at https://gitter.im/recogito/recogito-js](https://badges.gitter.im/recogito/recogito-js.svg)](https://gitter.im/recogito/recogito-js?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

## License

[BSD 3-Clause](LICENSE) (= feel free to use this code in whatever way
you wish. But keep the attribution/license file, and if this code
breaks something, don't complain to us :-)