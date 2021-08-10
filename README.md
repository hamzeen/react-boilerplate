# react-boilerplate

### scaffold

```sh
npx create-react-app react-boilerplate
cd react-boilerplate && npm install
```
```sh
echo "SKIP_PREFLIGHT_CHECK=true" > .env && open .env
npm start
```

## FUnctiona vs COmpo
unctional components are some of the more common components that will come across while working in React. These are simply JavaScript functions. We can create a functional component to React by writing a JavaScript function.
```js
import React ,{useState} from "react";
 
const FunctionalComponent=()=>{
    const[count , setCount]=useState(0);
 
    const increase=()=>{
        setCount(count+1);
    }
 
    return (
        <div style={{margin:'50px'}}>
            <h1>Welcome to Geeks for Geeks </h1>
            <h3>Counter App using Functional Componenet : </h3>
            <h2>{count}</h2>
            <button onClick={increase}>Add</button>
        </div>
    )
}
 
export default FunctionalComponent;
```

Compoennt 
```js
import React from "react";
 
class ClassComponent extends React.Component{
    constructor(){
        super();
        this.state={
            count :0
        };
        this.increase=this.increase.bind(this);
    }
     
   increase(){
       this.setState({count : this.state.count +1});
   }
 
    render(){
        return (
            <div style={{margin:'50px'}}>
               <h1>Welcome to Geeks for Geeks </h1>
               <h3>Counter App using Class Componenet : </h3>
               <h2> {this.state.count}</h2> 
               <button onClick={this.increase}> Add</button>
 
            </div>
        )
    }
}
 
export default ClassComponent;
```

### Create React App CRA:
create-react-app is the official CLI (Command Line Interface) for React to create React apps with no build configuration.

### React vs React Native
In Reactjs, virtual DOM is used to render browser code in Reactjs while in React Native, native APIs are used to render components in mobile.

### JSX
JSX is an XML-like syntax extension to ECMAScript without any defined semantics.

### PROPS vs STATE
The state is a data structure that starts with a default value when a Component mounts. It may be mutated across time, mostly as a result of user events.
Props (short for properties) are a Component’s configuration. Props are how components talk to each other. They are received from above component and immutable as far as the Component receiving them is concerned.


### Router
```sh
npm install --save react-router-dom
```

### JWT
* has 3 parts: header, payload & signature
* debug: jwt.io
* <https://gist.github.com/hamzeen/824761ffe3c605fa3c7ee270d871dc51>

### Typescript
* can be converted to TSX: <https://medium.com/@amcdnl/react-typescript-%EF%B8%8F-647aa7d054a9>
* not available out of the box through CRA (Create React App)

### JS Utils

```js
// translation from keys
const monthNames = {
  '1': 'Januari', '2': 'Februari', '3': 'March',
  '4': 'April', '5': 'Mei', '6': 'Juni',
  '7': 'Juli', '8': 'Augustus', '9': 'September',
  '10': 'Oktober', '11': 'Novemebr', '12': 'December'
}
const monthName = `month translation: ${monthNames[date.getMonth() + 1]}`;
```

```javascript
function sortByPriceAscending(jsonString) {
  const ary = JSON.parse(jsonString);
  return ary.sort(function(left, right) {
    return left.price - right.price;
  });
}

console.log(sortByPriceAscending('[
  {"name":"tea","price":1},
  {"name":"tomato","price":9.89},
  {"name":"sugar","price":4.04}
]'));
```

```javascript
// palindrome
const isPalindrome = (str) => 
    str.toLowerCase().split('').reverse().join('') === str.toLowerCase();
console.log(isPalindrome('rAceCar'));
```
```javascript
// date fromat dd-mm-yyyy
const now = new Date();
const date = now.toISOString().split('T')[0];
const newFormat = date.split('-').reverse().join('-');
console.log(newFormat):
```


### Extras
```css
// media query
@media (max-width: 1075px) {
  .container {
    margin: 40px;
  }
}

@media (max-width: 520px) {
  .container { margin: 40px 2px;}
}

// mixins: Mixins allow you to define styles that can be re-used throughout your stylesheet.

```

```sh
# file system (create with content):
echo "Hello World" > index.html && open index.html
```
* simple node server: 
```sh
npx http-server -a 0.0.0.0 -p 8000
```

* python: ```python -m SimpleHTTPServer 8000```
* npm dev dependency: ```npm install --save-dev {package@ver}```
* CURL:
```sh
curl -X POST 'http://localhost:8080/api/logs'
curl -I 'http://localhost:8080/api/logs'
```

### SCM
* remove all local changes:
```sh
git reset --hard HEAD
# work ...
git add .
git commit -m "messsage"
```

### REFERENCE: 
* Promises in the wild: https://davidwalsh.name/promises
* JWT: https://medium.com/@amcdnl/authentication-in-angular-jwt-c1067495c5e0
* UTIL: https://gist.github.com/hamzeen/52312f77aaa51bedbde7a48598c281d6
* UTIl 2: https://gist.github.com/hamzeen/e4516f7b580c6858c4136f688508014a
* https://www.youtube.com/watch?v=eofpZPRUnP8
* cal: https://github.com/usama093/Roman-Calculator/tree/19ad0bc8f010c9ea8329539095a2d5e7de87bb7a
