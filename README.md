# GitHub Activity

Two small HTML and JavaScript examples of HTTP **GET** requests.

## GitHub User Explorer

Download `github-user.html` and open it in a browser. Enter a GitHub username (the default is `C0mply`) and click one of the four buttons:

| Button | Public GitHub REST API endpoint |
| --- | --- |
| Followers | `https://api.github.com/users/{username}/followers` |
| Repos | `https://api.github.com/users/{username}/repos` |
| Events | `https://api.github.com/users/{username}/events/public` |
| Gists | `https://api.github.com/users/{username}/gists` |

The page shows readable results and the full JSON response. Each request uses `per_page=100&page=1`; a notice appears when another page is available. Events cover the public history available through GitHub's API.

The page handles empty results, unknown usernames, invalid input, request timeouts, and API rate limits. Changing the username clears old results; selecting another button cancels the previous request. No installation or token is required to read public data, but GitHub limits unauthenticated requests.

[GitHub REST API documentation](https://docs.github.com/en/rest)

## Original GET example

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
