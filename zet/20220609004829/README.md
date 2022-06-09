# React Customs Hooks
You can create a custom hook in react, to help you reuse some business logic through all of the website.
To do this you just define a const, as a convention any custom hook name should start with *use*.
Then you just write in whatever you want the hook to do and at the end return whatever you need to expose in order to
use your hook.
Ex:
```JS
const useCounter = (value) => {
    const [counter, setCounter] = useState(value);
    const increase = () => {
        setCounter(counter + 1);
    }
    return [counter, increase];
}
const App = () => {
    const [counter, increase] = useCounter(0);
    return (
        <div>
            Counter: {counter}
            <button onClick={increase}>Increase</button>
        </div>
    );
}
```
In the example we are creating a custom hook named *useCounter*. And to properly use the component we need to expose the counter (the actual value beign counted)
and the increase function (the function to call when wanting to increase the counter). Finally we use it as any other hook.

  #React #functionComponents #hooks #JS #coding 
