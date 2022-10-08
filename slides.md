---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: "text-center"
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: true
# some information about the slides, markdown enabled
info: |
  ## Basic Typescipt
# persist drawings in exports and build
drawings:
  persist: false
monaco: true
---

# Basic Typescript

<div class="text-white rounded-md  font-black">
  <span @click="$slidev.nav.next" class="bg-blue-500   rounded cursor-pointer p-3" hover="bg-black bg-opacity-10 text-blue-500">
  hands on experince on basic typescript features
  </span>
</div>

<div class="absolute ">
<img src="https://avatars.githubusercontent.com/u/66922536" class="max-w-36  rounded-full mx-auto ">
<p>
Saman Taghavi
</p>
</div>

<!--
Ask audience about their prior knowledge
-->

---

<h1 class="font-bold text-blue-500 text-xl">
 What is Typescript?
</h1>

TypeScript is JavaScript with syntax for types.

- 🐞 **Errors** - some of them can be noticed before deployment
- 🎨 **Tools** - most Editors support it and have tools for it
- 🧑‍💻 **Developer Experience** - if You know it well enough otherwise use any
  ```ts 
  let s: any = "I don't care enough";
  ```
- 🤹 **Inference** - Typescript understands JS, it can infer when possible
- 🎥 **Progressive** - we can add it, incrementally and opt-in

```ts {1|2,3|all}
// @ts-check
function oh(array) {
  if (orray.length > 0) {
    return array;
  }
}
```

<br>
<br>
<span class="bg-white bg-opacity-20 right-5 p-5 absolute rounded-md " hover="bg-opacity-70 text-black">
Read more about <a class="text-blue-500"  href='https://www.typescriptlang.org/docs/handbook/intro.html' target=”_blank”>
Typescript
</a>
</span>

<style>
h1 {
  background-color: blue;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>


---
layout: image-right
image: https://source.unsplash.com/collection/94734566/1920x1080
---

# Basic Types

see if you can solve this [simple problem](https://github.com/total-typescript/beginners-typescript-tutorial/blob/main/src/01-number.problem.ts#L11) from 
<br>
<br>

```ts {1-2|4-6|8-10|12-14|16-19|21-23|all} {maxHeight: '250px'}
// * 1. Boolean
var isDone = false;

// * 2. Number
var hex = 0xf00d;
var binary = 10;

// * 3. String
var color = "blue";
color = "red";

// * 4. Array
var list = [1, 2, 3];
var list2 = ["test", "not a test", "array of strings"];

// * 7. Any
var notSure: any = 4; // ? any type is given explicitly
notSure = "maybe a string instead";
notSure = false;

// * 9. Null and Undefined
let u = undefined;
let n = null;
```

later on we will try to solve more problems from [this repo](https://github.com/total-typescript/beginners-typescript-tutorial), shout out and thanks to [**@mattpocockuk**](https://twitter.com/mattpocockuk)


---
layout: image-left
image: https://source.unsplash.com/collection/94734566/1920x1080
---

# ENUMS

<br>
<br>
<br>

```ts 
type ColorEnum = "red" | "blue" | "green"; // ! one of the ways we can define a type

let ENUM_COLOR: ColorEnum = "blue"; // ! and use it
```


---
layout: cover
class: text-center
image: https://source.unsplash.com/collection/94734566/1920x1080
---

<div>
Thank you
</div>
