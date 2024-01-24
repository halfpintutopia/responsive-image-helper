# responsive-image-helper

## How to use

Ensure you have installed [`graphicsmagick`](http://www.graphicsmagick.org) or

```shell
brew install graphicsmagick
```

Globally install Grunt's CLI

```shell
npm install -g grunt-cli
```

Use NPM install packages

```shell
npm install 
```

Place images you wish to convert in the `src` directory. For every image, Grunt will generate images, in JPG and 
WebP format.

Currently, the compression is 80%, and the width ranges from 300 pixels to 4000 pixels.

To change the compression and width edit the following in `Gruntfile.js`.

```javascript
sizes: [{
            name: "xs",
            suffix: "_1x",
            quality: 80,
            width: 300
        },
        {
            name: "xs",
            suffix: "_2x",
            quality: 80,
            width: 600
        },
        {
            name: "sm",
            suffix: "_1x",
            quality: 80,
            width: 800
        },
        {
            name: "sm",
            suffix: "_2x",
            quality: 80,
            width: 1600
        },
        {
            name: "md",
            suffix: "_1x",
            quality: 80,
            width: 1000
        },
        {
            name: "md",
            suffix: "_2x",
            quality: 80,
            width: 2000
        },
        {
            name: "lg",
            suffix: "_1x",
            quality: 80,
            width: 1200
        },
        {
            name: "lg",
            suffix: "_2x",
            quality: 80,
            width: 2400
        },
        {
            name: "xl",
            suffix: "_1x",
            quality: 80,
            width: 2000
        },
        {
            name: "xl",
            suffix: "_2x",
            quality: 80,
            width: 4000
        },
    ]
```


## References

- [A Guide to Responsive Images with Ready-to-Use Templates](https://medium.com/free-code-camp/a-guide-to-responsive-images-with-ready-to-use-templates-c400bd65c433)
