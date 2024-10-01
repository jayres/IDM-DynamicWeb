# Exercise Three: Weather App

## Requirements:

1. Github
2. Everything from Exercise One and Two

## Directions:

1. Create new Github Repository named "Dynamic Web Exercise Three"

2. Create new Next.js project

```
npx create-next-app@latest
```

`no, yes, no, no, yes, no`

3. Init new Github repo inside of the new project

4. We will use the default page.js only

- page.js (home page)
- (optional) Clean out files you are not going to use

6. Create components for injesting data in a `components` folder (/src/app/components)

### 7. Setting up Weather API

- Go to [https://openweathermap.org/guide](https://openweathermap.org/guide) and follow the directions
- [https://home.openweathermap.org/users/sign_up](https://home.openweathermap.org/users/sign_up) create a new account (use your school address and you won't have to pay anything)
- When logged in, go to [API Keys](https://home.openweathermap.org/api_keys) and either create a key or use one that may be there
- Store your key somewhere (in the code as per my instructions) as [an environmental variable](https://nextjs.org/docs/pages/building-your-application/configuring/environment-variables)

10. Setup a query based on a city per the OpenWeatherMap docs [https://openweathermap.org/current](https://openweathermap.org/current)

11. Display:

- Weather Type (ex. Cloudy)
- Current Temperature
- High Temperature
- Low Temperature
- Cloudiness
- Humidity
- Wind Speed

12. Setup URL Queries for different cities (at least 4 cities)

13. Display image based on weather type

14. Set background color based on cloudiness (or temperature if you want)

15. Style the page so it has a unique look and has a responsive layout

16. Submit the link to the Github repo _AND a screenshot of your weather app_ to James at ja155@nyu.edu

## Useful Resources

[OpenWeather API](https://openweathermap.org/current)

[Pre-rendering and Data Fetching - Next](https://nextjs.org/learn/basics/data-fetching/getstaticprops-details)

[Next.js getStaticPaths](https://nextjs.org/docs/pages/building-your-application/data-fetching/get-static-paths) - You will need this when you use getStaticProps and dynamic URLs like we are.

[Fetch - MDN](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)

[useState](https://reactjs.org/docs/hooks-reference.html#usestate)

[useEffect](https://reactjs.org/docs/hooks-reference.html#useeffect)

[Switch statements](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/switch)

[FontAwesome](https://www.npmjs.com/package/@fortawesome/react-fontawesome)

[FontAwesome Weather Icons](https://fontawesome.com/icons?d=gallery&c=weather&m=free)

[Next.js](https://nextjs.org/docs)

[Routing in Next.js](https://nextjs.org/docs/app/building-your-application/routing)

Please note that this is for a different _methodology_ of React that we are going to be using for this class - it is instructive though and should help you understand some more in depth things.

[Next.js Page Routing](https://nextjs.org/docs/pages/building-your-application/routing/pages-and-layouts)

[Next.js Links](https://nextjs.org/docs/pages/building-your-application/routing/linking-and-navigating)

[Next.js Env Vars](https://nextjs.org/docs/pages/building-your-application/configuring/environment-variables)

[Openweather Weather Types](https://openweathermap.org/weather-conditions)
