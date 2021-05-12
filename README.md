# react-boilerplate

### scaffold

```
npx create-react-app react-boilerplate
cd react-boilerplate && npm install
```
```
echo "SKIP_PREFLIGHT_CHECK=true" > .env && open .env
npm start
```

### JWT
* has 3 parts: header, payload & signature
* debug: jwt.io
* <https://gist.github.com/hamzeen/824761ffe3c605fa3c7ee270d871dc51>

### Typescript
* can be converted to TSX: <https://medium.com/@amcdnl/react-typescript-%EF%B8%8F-647aa7d054a9>
* not available out of the box through CRA (Create React App)

### JSON Obj: translation
```
const monthNames = {
  '1': 'Januari', '2': 'Februari', '3': 'March',
  '4': 'April', '5': 'Mei', '6': 'Juni',
  '7': 'Juli', '8': 'Augustus', '9': 'September',
  '10': 'Oktober', '11': 'Novemebr', '12': 'December'
}
const monthName = `month translation: ${monthNames[date.getMonth() + 1]}`;
```

### Extras
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
