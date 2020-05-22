# TEST_DATA

This repository is used for retrieving data from a backend. These are the entities:
* [hall](https://my-json-server.typicode.com/RALGIE/TEST_DATA/hall)  
* [performance](https://my-json-server.typicode.com/RALGIE/TEST_DATA/performance)
* [artist](https://my-json-server.typicode.com/RALGIE/TEST_DATA/artist)

## curl

```bash
curl --header \
  "Content-Type: application/json" \
  --request POST \
  --data '{"id": 4,"title":"new title"}' \
  https://my-json-server.typicode.com/RALGIE/TEST_DATA/performance

```

## Javascript

This API does't store the data. Because it is a online JSON server. When you host the data locally the data is seved to your locale server.

```javascript
  fetch('https://jsonplaceholder.typicode.com/RALGIE/TEST_DATA/performance', {
    method: 'POST',
    body: JSON.stringify({
      title: 'foo',
      seats_taken: 2
    }),
    headers: {
      "Content-type": "application/json; charset=UTF-8"
    }
  })
  .then(response => response.json())
  .then(json => console.log(json))
  ```
