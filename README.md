when use `?raw` to import a module, vite:define plugin should skip replacement.
run `yarn build`

source code
```javascript
import './style.css'
import md from './index.md?raw'

document.getElementById('app').innerHTML = md

```

after build:
```javascript
document.getElementById("app").innerHTML=NaN;

```
