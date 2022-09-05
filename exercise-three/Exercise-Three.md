# Exercise Three: Weather App

## Requirements:

1. Use Github better
2. Everything from Exercise One

## Directions:

1. Create new Github Repository named "Dynamic Web Exercise Two"

2. Install Create React App and Create New Project

```
npx create-react-app exercise-two
```

(note, you may have to install npx: `npm install -g npx`)

3. Init new Github repo inside of the new project

4. Add the following packages through npm:

- React Router `npm install react-router`
- React Router DOM `npm install react-router-dom`

5. Create one page inside a `containers` folder

- Home page
- Clean out files you are not going to use

6. Create components for injesting data in a `components` folder

### 7. Setting up Weather API

- Go to [https://openweathermap.org/guide](https://openweathermap.org/guide) and follow the directions
- [https://home.openweathermap.org/users/sign_up](https://home.openweathermap.org/users/sign_up) create a new account (use your school address and you won't have to pay anything)
- When logged in, go to [API Keys](https://home.openweathermap.org/api_keys) and either create a key or use one that may be there
- Store your key somewhere (in the code as per my instructions)

9. Install Axios `npm install axios`

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

16. Submit the link to the Github repo AND a screenshot of your weather app to James at ja155@nyu.edu

## Useful Resources

[Create React App](https://github.com/facebook/create-react-app)

[React Router](https://www.npmjs.com/package/react-router)

[Getting an ID from the URL](https://tylermcginnis.com/react-router-url-parameters/)
Please note that this is for a different _methodology_ of React that we are going to be using for this class - it is instructive though and should help you understand some more in depth things.

[OpenWeather API](https://openweathermap.org/current)

[Axios](https://www.npmjs.com/package/axios)

[URLSearchParams](https://developer.mozilla.org/en-US/docs/Web/API/URLSearchParams)

[useState](https://reactjs.org/docs/hooks-reference.html#usestate)

[useEffect](https://reactjs.org/docs/hooks-reference.html#useeffect)

[Switch statements](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/switch)

[FontAwesome](https://www.npmjs.com/package/@fortawesome/react-fontawesome)

[FontAwesome Weather Icons](https://fontawesome.com/icons?d=gallery&c=weather&m=free)
