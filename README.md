# &lt;google-adsense&gt;
==============

Web Component wrapper for Google Adsense code using [Polymer](http://polymer-project.org).
> Maintained by [Kessiler Rodrigues](https://github.com/kessiler).


## Demo

[Check it live!](http://kessiler.github.io/google-adsense)

## Install

Install the component using [Bower](http://bower.io/):

```sh
$ bower install google-adsense --save
```

Or [download as ZIP](https://github.com/kessiler/google-adsense/archive/master.zip).

## Usage

1. Import Web Components' polyfill:

    ```html
    <script src="bower_components/platform/platform.js"></script>
    ```

2. Import Google Adsense custom element:

    ```html
    <link rel="import" href="bower_components/google-adsense/dist/google-adsense.html">
    ```

3. Start using it!

    ```html
    <google-adsense></google-adsense>
    ```
    
    
## Options

Attribute     | Options     | Default             | Description
---           | ---         | ---                 | ---
`client`      | *int*       | `8949501714982201`  | your id from ad.
`slot`        | *int*       | `2732884579`        | number of slot ad.
`width`       | *int*       | `728`               | width size of ad.
`height`      | *int*       | `90`                | height size of ad.


## Responsive

To make the ad responsive, you must create media queries for the class "ads-responsive".

* Example

    ```sh
    @media(min-width: 320px) { .ads-responsive { width: 300px; height: 250px; } }
    @media(min-width: 500px) { .ads-responsive { width: 468px; height: 60px; } }
    @media(min-width: 800px) { .ads-responsive { width: 728px; height: 90px; } }
    ```

## Development

In order to run it locally you'll need to fetch some dependencies and a basic server setup.

* Install [Bower](http://bower.io/) & [Grunt](http://gruntjs.com/):

    ```sh
    $ [sudo] npm install -g bower grunt-cli
    ```

* Install local dependencies:

    ```sh
    $ bower install && npm install
    ```

* To test your project, start the development server and open `http://localhost:8000`.

    ```sh
    $ grunt server
    ```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## License

[MIT License](http://opensource.org/licenses/MIT)
