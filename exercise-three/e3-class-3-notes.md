# What we will do this class:

1. Update getStaticProps to have params

- We can query based on the param and we give a default value.
- Ensure the `q=` has the dynamic parameter
- We are destructuring a single agument that `getStaticProps` accepts

```js
export async function getStaticProps({ params }) {
  const city = (params && params.city) || "Boston";
    const res = await fetch(
    `https://api.openweathermap.org/data/2.5/weather?q=${city}&appid=${process.env.WEATHER_API_KEY}&units=imperial`
  );
  ...
```

2. Add getStaticPaths:

- Next.js way of ensuring you have a list of paths to generate static
- This is a deeper level of abstraction than we will dive into in
  this class

```js
export const getStaticPaths = async () => {
  return {
    paths: [],
    fallback: true,
  };
};
```

3. Change pages/index.js to `[[...city]].js`

- Allows us to get the city param
- The elipses is Next.js's way of allowing for empty/absent params
  to a default.

4. Add if data is undefined check to your Home function

```js
export default function Home({ weatherData }) {
  if (!weatherData) return null;
  return (
    ...
```

5. Added Header to link to a query for individual cities
