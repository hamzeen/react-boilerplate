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
* has 3 parts: header, body & signature
* debug: jwt.io

### Typescript
* can be converted to TSX: <https://medium.com/@amcdnl/react-typescript-%EF%B8%8F-647aa7d054a9>
* not available out of the box through CRA (Create React App)


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
* https://www.youtube.com/watch?v=eofpZPRUnP8
