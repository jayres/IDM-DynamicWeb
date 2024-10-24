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
async function Page() {
  const FIRST_API = `https://api.whatever.com`;
  const responseFirstAPI = await fetch(FIRST_API);
  const firstAPIData = await responseFirstAPI.json();
  const valueNeededForSecondAPI = firstAPIData.coolValue;

  const SECOND_API = `https://api.yeah.com/${valueNeededForSecondAPI}`;
  const responseSecondAPI = await fetch(SECOND_API);
  const secondAPIData = await responseSecondAPI.json();

  return (
    <div>
      {secondAPIData.map((data) => (
        <p>{data.valueFromThisData}</p>
      ))}
    </div>
  );
}
```

# Querying an API with Headers

Headers are data that are sent in the request to the API.
Previously we have used URL parameters to send this data but many APIs require the data be sent as a header.

The way to use headers can be found [in the fetch MDN](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API).

```js
const url = `https://api.whatever.com`;
const bearerToken = `Bearer ${process.env.API_KEY}`;

const response = await fetch(url, {
  method: "POST",
  headers: {
    Authorization: bearerToken,
    "Content-Type": "application/json",
  },
});
```

# Using JSON Data with an API

If you are unable to find a second remote API that makes sense you may use a JSON file that you find or make (similar to exercise two).

## Valid JSON format

Below is some sample JSON to demonstrate some different patterns you may see. Ultimately remember that it is an array of objects and objects have key/value pairs.

```json
[
  {
    "key": "value",
    "key2": [
      {
        "key3": 1000
      }
    ]
  }
]
```

## Using JSON data

Just like with Exercise Two, you can import the data and use it inside of the React component. In the example below I am using an ID I got from another API request to find a specific piece of JSON data.

```jsx
import jsonData from "../jsonData";

async function Page() {
  const FIRST_API = `https://api.whatever.com`;
  const responseFirstAPI = await fetch(FIRST_API);
  const firstAPIData = await responseFirstAPI.json();
  const idForJSONData = firstAPIData.id;

  // Find is an array method to search through an array and return
  // the place in the array where the arrow function returns true.
  // 'data' in the opening parenthesis represents the element in the
  // array at the current index. This can be named anything.
  const jsonInformationToUse = jsonData.find(
    (data) => data.id === idForJSONData
  );

  return (
    <div>
      <p>{jsonInformationToUse.whateverInfoInMyFile}</p>
    </div>
  );
}
```
