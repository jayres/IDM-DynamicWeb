# Sample Code for Midterm Project

## Querying Two APIs

```js
const FIRST_API = `https://api.whatever.com`;
const SECOND_API = `https://api.yeah.com`;
// Just like exercise three...
export async function getStaticProps() {
  // Get first API query
  const responseFirstAPI = await fetch(FIRST_API);
  const firstAPIData = await responseFirstAPI.json(); // This might be different for each API
  // Get second API query
  const responseSecondAPI = await fetch(SECOND_API);
  const secondAPIData = await responseSecondAPI.json(); // This might be different for each API
  // Pass the responses down as props
  return {
    props: {
      firstAPIData,
      secondAPIData,
    },
  };
}
```

## Querying Two APIs that interact with one another

```js
export async function getStaticProps() {
  // Get first API query
  const responseFirstAPI = await fetch(FIRST_API);
  const firstAPIData = await responseFirstAPI.json();
  // Is there some data you need from the first API to get data from the second API?
  const valueINeed = firstAPIData.whatever.thing;
  const anotherValueINeed = firstAPIData.hmm.yes;
  // Get second API query with value from first API
  const responseSecondAPI = await fetch(
    `https://api.whatever.com/posts?value=${valueINeed}&another=${anotherValueINeed}`
  );
  const secondAPIData = await responseSecondAPI.json();
  // Pass the responses down as props
  return {
    props: {
      firstAPIData, // If you need to pass the first API data...
      secondAPIData,
    },
  };
}
```
