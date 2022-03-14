# world-countries-list (Stencil Component)

# NOTE

## Installation

To install, you can use [npm](https://npmjs.org/) or [yarn](https://yarnpkg.com):


    $ npm install --save world-countries-list
    $ yarn add world-countries-list
    
Once Installed please add the below custom elements in your react-app or angular-app

1. index.js

import { defineCustomElements } from "world-countries-list/loader"
defineCustomElements(window);

2. In your App Conmponent or Custom Component , Please add the below custom element
            <countries-list></countries-list>


## Examples

Here is a simple example of world-countries-list being used in an react app:


```jsx index.js
import reportWebVitals from './reportWebVitals';
import { defineCustomElements } from "world-countries-list/loader"
const store = createStore(rootreducer, applyMiddleware(thunk));

ReactDOM.render(
  <React.StrictMode>
    <Provider store={store}><Router /></Provider>
  </React.StrictMode>,
  document.getElementById('root')
);

// If you want to start measuring performance in your app, pass a function
// to log results (for example: reportWebVitals(console.log))
// or send to an analytics endpoint. Learn more: https://bit.ly/CRA-vitals
reportWebVitals();
defineCustomElements(window);

App.js

function App() {
  
  return (
    <div>
      <button onClick={openModal}>Open Modal</button>
      <countries-list></countries-list>
    </div>
  );
}

ReactDOM.render(<App />, appElement);

You can find more examples in the `examples` directory, which you can run in a
local development server using `npm start` or `yarn run start`.

## Explanantion
<countries-list> ## This component will get list of countries in array from external API and stored it in your 
browser session storage.

