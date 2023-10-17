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
