# Hyper Lazyload

Simple lazy loading of images with minimal markup changes.

### Installing

In your project directory:

```
npm install hyper-lazyload
```

### Usage

In your project HTML file make a container to hold images and assign an ID:

``` 
    <body>
        <div id="lazy-load">
        </div>
    </body>
```

In your project JS file:

```
import lazyload from 'hyper-lazyload'

/**
 * Initialize the lazyloading on a container
 * @param {images} Array<string> of your images
 * @param {chunk} [c=3] any number, defaults to 3
 * @param {containerId} string for the id of your container, defaults to 'lazy-load'
 * @param {throttleDuration} any int number, sets the duration of the scroll throttling * defaults to an integer of 1000
 */

lazyload.init(
    ['/image1.jpg', '/image2.jpg'],
    3,
    'lazy-load',
    1000
)

```

## Running the tests

`npm run test`

## License

MIT