# steerableStorage

A easy web storage manager;

## Install

```bash
npm install steerableStorage --save
```



## Usage 

```js
import SteerableStorage from 'steerable-storage'

const storage = new SteerableStorage('localStorage', 'projectName')

// add or update storage
storage.getItem('key', 'value')

// remove storage
storage.removeItem('key')

// clear all project storage
storage.clear()

// view all valid storage
storage.values
```



## Arguments

| params  | type          | required | default               | options                          |
| ------- | ------------- | -------- | --------------------- | -------------------------------- |
| storage | string        | true     |                       | 'localStorage'、'sessionStorage' |
| namespace  | string        | true     |                       |                                  |
| expires | number        | false    | 1000 * 3600 * 24 * 30 |                                  |
| version | number/string | false    | 1                     |                                  |

