# Built-in React Hooks

[Link to documentation](https://react.dev/reference/react/hooks)

## useState

```js
const [stateValue, setStateValueFunction] = useState("Hmm");

return (
  <div>
    {stateValue}
    <button onClick={() => setStateValFunc("hello")}>Set Hello</button>
    <button onClick={() => setStateValFunc("bye")}>Set Bye</button>
  </div>
);
```

## useEffect

```js

const [dataValues, setDataValues] = useState()
const needToUpdate = 'this is a value that when it will update the useEffect will run again'

useEffect(
  () => {
    const response = await fetch('this')
    setDataValues(response.tojson())
  },
  [needToUpdate]
)

```

## useCallback

```js
const [dataToDisplay, setDataToDisplay] = useState([]);

const getNewData = useCallback(async () => {
  const response = fetch();
  // do whatever I want here...
  setDataToDisplay(response.tojson());
}, []);

return (
  <div>
    {dataToDisplay}
    <button onClick={() => getNewData()}>New Data</button>
  </div>
);
```

## useMemo

```js
const value = useMemo(() => {
  return horses;
}, [horses]);

const { valueOne, valueTwo } = useMemo(() => {
  if (horses === "yes") {
    return {
      valueOne: "hay",
      valueTwo: currentBarn,
    };
  }
  return {
    valueOne: "no hay",
    valueTwo: "no barn",
  };
}, [currentBarn, horses]);
```
