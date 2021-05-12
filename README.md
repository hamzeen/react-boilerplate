# react-boilerplate

### JSX
JSX is an XML-like syntax extension to ECMAScript without any defined semantics.

### scaffold

```
npx create-react-app react-boilerplate
cd react-boilerplate && npm install
```
```
echo "SKIP_PREFLIGHT_CHECK=true" > .env && open .env
npm start
```

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
* file system (create with content): 
```sh
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
* JWT: https://medium.com/@amcdnl/authentication-in-angular-jwt-c1067495c5e0
* UTIL: https://gist.github.com/hamzeen/52312f77aaa51bedbde7a48598c281d6
* UTIl 2: https://gist.github.com/hamzeen/e4516f7b580c6858c4136f688508014a
* https://www.youtube.com/watch?v=eofpZPRUnP8
