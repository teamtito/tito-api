# tito-api
[![NPM](https://nodei.co/npm/tito-api.png)](https://nodei.co/npm/tito-api/)

Node: In Development for the v2 API.

Node client for the http://tito.io api.

## usage

```js
var tito = require('tito-api')

var t = tito('YOUR_API_KEY') // find it here https://api.tito.io/

t.tickets().on('data', function (ticket) {
  console.log(ticket.name)
})
```

## endpoints

### t.tickets()
All tickets of all events
returns readable object stream

### t.events()
All events.
returns readable object stream

### t.accounts()
All accounts granted access to.
returns readable object stream

### t.request(endpoint)

endpoints e.g. an event like `nodeschool-berlin/12`

return readable unparsed stream
