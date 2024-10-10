# Sample Code for Midterm Project

## Querying Two APIs

```js
const FIRST_API = `https://api.whatever.com`;
const SECOND_API = `https://api.yeah.com`;
// Just like exercise three...

// Get first API query
const responseFirstAPI = await fetch(FIRST_API);
const firstAPIData = await responseFirstAPI.json(); // This might be different for each API
// Get second API query
const responseSecondAPI = await fetch(SECOND_API);
const secondAPIData = await responseSecondAPI.json(); // This might be different for each API
```

## Querying Two APIs that interact with one another

```js
// Incoming
```

# Querying an API with Headers

Headers are data that are sent in the request to the API.
Previously we have used URL parameters to send this data but many APIs require the data be sent as a header.

The way to use headers can be found [in the fetch MDN](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API).

```js
const bearerToken = `Bearer ${process.env.API_KEY}`;
const response = await fetch(url, {
  method: "POST",
  headers: {
    Authorization: bearerToken,
    "Content-Type": "application/json",
  },
});
```
