## mongoose-attachments-aws2js

S3 Storage Provider for [mongoose-attachments](https://github.com/firebaseco/mongoose-attachments) backed by the [Amazon Web Services node.js module](https://github.com/SaltwaterC/aws2js).

### Installation

    $ npm install mongoose-attachments-aws2js

### Usage

The library will register automatically with `mongoose-attachments` by performing `require` and
return a reference to the mongoose-attachments plugin:

    var attachments = require('mongoose-attachments-aws2js');

For further instructions check [mongoose-attachments](https://github.com/firebaseco/mongoose-attachments).

### Provider Configuration
#### Provider Name:

    aws2js

#### Configuration properties

    providerName: 'aws2js',
    options: {
      key: '<key>',
      secret: '<secret>',
      bucket: '<bucket>',
      endpoint: 'https://' + options.bucket + '.s3.amazonaws.com',
      acl: "public-read" // false or "private" by default
    }

`endpoint` is optional and defaults to `'https://' + options.bucket + '.s3.amazonaws.com'`.
`acl` is by default `false` or `private`. If you don't want to create complex s3 policies to download the files then use `public-read`.

For other configurations check [mongoose-attachments](https://github.com/firebaseco/mongoose-attachments).

### Contributors

* [Firebase.co](https://github.com/firebaseco)
* [Chantal Ackermann](https://github.com/nuarhu)

## License (MIT)

Copyright (c) 2011-2013 Firebase.co - http://firebase.co

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

