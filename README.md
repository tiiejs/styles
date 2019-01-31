## Tiiejs loader
Basic style for tiiejs.

## Install

### Webpack

First we need to define alias for Webpack.

```js
// webpack.config.js

const path = require('path');

module.exports = (environment) => {
    return {
        // ...
        resolve : {
            alias : {
                // ...
                "Tiie/Styles" : "tiiejs-styles/src",
                "Tiie" : "tiiejs/src",
            }
        }
    }
};
```

Then plug extension.

```js
import App from "Tiie/App";
import extensionStyles from "Tiie/Styles/extension"

// ...
let app = new App(jQuery("body"));

app.plugin(extensionStyles);
app.run();
```

**The documentation is being created ...**
