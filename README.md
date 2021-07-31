# Firebase Auth Error Codes in English

## Usage

```js
const firebaseErrors = require('./error_codes.json'); 

export function localizeErrorMap(e?: Error & { code?: string }) {
  if (typeof e === 'object' && typeof e.code === 'string' && e.code in firebaseErrors)
    e.message = (firebaseErrors as any)[e.code];
}
```
