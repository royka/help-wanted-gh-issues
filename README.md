# help-wanted-gh-issues

An element providing a starting point for your own reusable Polymer elements.


## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install


## Playing With Your Element

If you wish to work on your element in isolation, we recommend that you use
[Polyserve](https://github.com/PolymerLabs/polyserve) to keep your element's
bower dependencies in line. You can install it via:

    npm install -g polyserve

And you can run it via:

    polyserve

Once running, you can preview your element at
`http://localhost:8080/components/help-wanted-gh-issues/`, where `help-wanted-gh-issues` is the name of the directory containing it.

## Installing the Element to use in another project

Install with bower

    bower install help-wanted-gh-issues --save

Include shim and html in `index.html`

    <script src="./bower_components/webcomponentsjs/webcomponents-lite.min.js"></script>
    <link rel="import" href="./bower_components/help-wanted-gh-issues/help-wanted-gh-issues.html">

Use it

    <help-wanted-gh-issues owner='bower'repo='bower'></help-wanted-gh-issues>


## Testing Your Element

Simply navigate to the `/test` directory of your element to run its tests. If
you are using Polyserve: `http://localhost:8080/components/help-wanted-gh-issues/test/`

### web-component-tester

The tests are compatible with [web-component-tester](https://github.com/Polymer/web-component-tester).
Install it via:

    npm install -g web-component-tester

Then, you can run your tests on _all_ of your local browsers via:

    wct

#### WCT Tips

`wct -l chrome` will only run tests in chrome.

`wct -p` will keep the browsers alive after test runs (refresh to re-run).

`wct test/some-file.html` will test only the files you specify.


## Yeoman support

If you'd like to use Yeoman to scaffold your element that's possible. The official [`generator-polymer`](https://github.com/yeoman/generator-polymer) generator has a [`seed`](https://github.com/yeoman/generator-polymer#seed) subgenerator.
