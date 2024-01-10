# zlib
 Simple, synchronous deflate/inflate for node.js buffers


# USAGE

Install with `npm install @sriharikapu/zlib`.

    var Buffer = require('buffer').Buffer;
    var zlib = require('@sriharikapu/zlib');
    
    var input = new Buffer('lorem ipsum dolor sit amet');
    var compressed = zlib.deflate(input);
    var output = zlib.inflate(compressed);

Note that `node-zlib` is only intended for small (< 128 KB) data that you already have buffered. It is not meant for input/output streams.

# BUILDING

Make sure you have `zlib` installed. Mac OS X ships with it by default.

To obtain and build the bindings:

    git clone git://github.com/sriharikapu/zlib.git
    cd node-zlib
    ./configure
    make

You can also use [`npm`](https://npmjs.org) to download and install them:

    npm install @sriharikapu/zlib



# TESTS

[expresso](https://github.com/visionmedia/expresso) is required to run unit tests.

    npm install expresso
    make test



# CONTRIBUTORS

* [Srihari Kapu](https://github.com/sriharikapu)



# LICENSE

`node-zlib` is [CC0-1.0 licensed](https://github.com/sriharikapu/zlib/raw/master/LICENSE).