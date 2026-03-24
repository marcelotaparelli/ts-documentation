# Typescript Documentation
<br><br>

## Playground for .d.ts
https://www.typescriptlang.org/play
<br><br>

## .d.ts Modules

Are declarative files that describe the shape of JS modules.

```javascript
// .js code

let result = myLib.makeGreeting("hello, world");
console.log("The computed greeting is:" + result);
let count = myLib.numberOfGreetings;
```
<br><br>

```typescript
// .d.ts 

declare namespace myLib {
  function makeGreeting(s: string): string;
  let numberOfGreetings: number;
}
```
