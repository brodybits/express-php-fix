# express-php-fix

Serving PHP over Express & Node.js, with a fix for a user-specified `php-cgi` command.

## Example

```js
var express = require('express');
var php = require('express-php');
var app = express();

app.use(php.cgi('./httpdocs', '/usr/local/bin/php-cgi'));
app.use(express.static('./httpdocs'));

app.listen(4000);
```

## Installation

```bash
$ npm install express-php
```

php-cgi should be installed, if not:
```bash
$ sudo apt-get install php5-cgi
```

## Compiling coffee2js

```bash
$ npm install -g coffee-script
$ coffee -b -c index.coffee
```

## License

  [MIT](LICENSE)
