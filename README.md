# TEST_DATA

This repository is used for retrieving data from a backend. These are the entities:
* hall
* performance
* artist
* posts
* comments

## curl

```bash
curl --header \
  "Content-Type: application/json" \
  --request POST \
  --data '{"id": 4,"title":"new title"}' \
  https://my-json-server.typicode.com/RALGIE/TEST_DATA/posts

```

## Javascript

This API does't store the data. Because it is a online JSON server. When you host the data locally the data is seved to your locale server.

```javascript
  fetch('https://jsonplaceholder.typicode.com/posts', {
    method: 'POST',
    body: JSON.stringify({
      title: 'foo',
      body: 'bar',
      userId: 1
    }),
    headers: {
      "Content-type": "application/json; charset=UTF-8"
    }
  })
  .then(response => response.json())
  .then(json => console.log(json))
  ```
