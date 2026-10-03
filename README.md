# GitHub Activity

A small HTML and JavaScript example of an HTTP **GET** request.

## Sample link

[GET https://jsonplaceholder.typicode.com/posts/1](https://jsonplaceholder.typicode.com/posts/1)

## Run

Download `index.html` and open it in a browser. Click **Send GET request** to retrieve a post and display its JSON response and HTTP status. An internet connection is required.

The page also includes a direct sample link, error handling, and a 10-second request timeout. No installation or API key is required.

## Request

```javascript
fetch('https://jsonplaceholder.typicode.com/posts/1', {
  method: 'GET',
  headers: { Accept: 'application/json' }
});
```

[API documentation](https://jsonplaceholder.typicode.com/)

The repository's existing `LICENSE` applies to this code.
