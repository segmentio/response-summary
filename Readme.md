# response-summary

    Return a response summary.

## Example

```js
var Summary = require('response-summary');

var app = express();
app.get(function (req, res, next) {
    var summary = Summary(req, res);
    console.log('Bytes sent: ' + summary.bytesSent);
    next();
});
```

## API

### .summary(req, res)
    
    Return an object summarizing a response.