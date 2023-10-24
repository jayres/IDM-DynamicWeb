# useState

```js
const [stateValue, setStateValueFunction] = useState("Hmm");

return (
  <div>
    {stateValue}
    <button onClick={() => setStateValueFunction("hello")}>Hello</button>
    <button onClick={() => setStateValueFunction("goodbye")}>Goodbye</button>
  </div>
);
```

# useEffect

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

# useCallback

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
