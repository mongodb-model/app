# DB Query

 Standalone base module extending the NodeJs Transform API with few other functionalities added

### Installation

```bash
$ yarn add @mongodb-model/app 

```
 or 

```bash

$ npm i @mongodb-model/app

```

### Simple Usage Example

```bash
 const Base = require('@mongodb-model/app');
 const base = new Base();
 base.apiGet();
 base.on('apiGet', data => console.log(data));
 base.on('apiGet-error', error => console.error(error));
 
```
or 
```bash
 class MyWonderfulClass extends require('@mongodb-model/app') {

    constructor(...arrayOfObjects) {

    super({ objectMode: true, encoding: "utf-8", autoDestroy: true });

    arrayOfObjects.forEach(option => {
        if(Object.keys(option).length > 0){
            Object.keys(option).forEach((key) => { if(!this[key]) this[key] = option[key];})
        }
    });

    this.autobind(MyWonderfulClass);
    this.autoinvoker(MyWonderfulClass);
    this.setMaxListeners(Infinity);
  }
 };
 
```

