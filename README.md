# Ngv16Reproduction

```sh
npm i
ng serve
```

you'll see:
<img width="1649" alt="CleanShot 2023-07-25 at 13 33 07@2x" src="https://github.com/sod/ng16-issue-throwing-syntax/assets/905328/73276ba9-edb8-421b-b48f-1ffc05e1bf4d">

And the watcher won't recover.

Issue caused by this typescript code:

```ts
function foo(): {[foo: number] {}
```
