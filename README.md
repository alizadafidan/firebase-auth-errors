# Firebase Auth Error Codes in English

## Usage

```js
export function localizeErrorMap(e?: Error & { code?: string }) {
  if (typeof e === 'object' && typeof e.code === 'string' && e.code in firebaseErrors)
    e.message = (firebaseErrors as any)[e.code];
}
```
