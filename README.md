# Typescript Documentation
<br><br>

## Playground for .d.ts
https://www.typescriptlang.org/play
<br><br>

## .d.ts Modules
- Are declarative files that describe the shape of JS modules.

```javascript
// .js code

let result = myLib.makeGreeting("hello, world");
console.log("The computed greeting is:" + result);
let count = myLib.numberOfGreetings;
```
<br>

```typescript
// .d.ts 

declare namespace myLib {
  function makeGreeting(s: string): string;
  let numberOfGreetings: number;
}
```
<br><br>

## Declaration Merging
- It's when the compliler merges two separate declaration with the same name into a single one.

```typescript
interface Box {
  height: number;
  width: number;
}
interface Box {
  scale: number;
}
let box: Box = { height: 5, width: 6, scale: 10 };

// You can extend existing @types:

declare namespace Express {
  interface Request {
    user?: {
      userId: string;
      email: string;
    }
  }
}
```
