# VITE Example project create React App

1. npm create vite@latest vite-app [select React -> Javascript]
2. cd vite-app
3. code .
4. install library.

```
$ npm i
```
   
5. config vite

```javascript
// open vite.config.js
// add line to

export default defineConfig({
  plugins: [react()],
  server: {
    port: 3000,
  }
})
```
6. add .env file and add this line 

``` 
VITE_API_URL=http://localhost:3000
```

7. create components folder and Header.jsx inside folder and code.

```javascript
const Header = () => {
    return <div>{ import.meta.env.VITE_API_URL }</div>;
}

export default Header;
```

8. open App.jsx file and import Header and insert Header tag.

``` javascript
import Header from './components/Header'
...
...
    <div className="App">
        <Header />

...
...

```

9. run app.

```
    $ npm run dev // for dev server.
    $ npm run build // for build production files.
    $ npm run preview // for preview production mode from dist folder.
```
