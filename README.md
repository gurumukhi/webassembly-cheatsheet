# WebAssembly Cheatsheet

## What is WebAssembly?
* WebAssembly (also known as WASM) is a new type of code that can be run in modern web browsers. 
* It is a low-level assembly-like language with a compact binary format that runs with near-native performance and provides languages such as C/C++ and Rust with a compilation target so that they can run on the web.
* It is also designed to run alongside JavaScript, allowing both to work together.

## How does WebAssembly fit into the web platform?
The web platform can be thought of as having two parts:
1. A virtual machine (VM) that runs the Web app’s code, e.g. the JavaScript code that powers your apps.
2. A set of Web APIs that the Web app can call to control web browser/device functionality and make things happen (DOM, CSSOM, WebGL, IndexedDB, Web Audio API, etc.).

With the advent of WebAssembly appearing in browsers, the virtual machine mentioned in (1) above will now load and run two types of code — JavaScript AND WebAssembly.

## Try WebAssembly:
Find the instructions at developers guide at  https://webassembly.org/getting-started/developers-guide/

## Key features of WebAssembly:
WebAssembly enables near-native performance for games and apps
* Fast start times (smaller download and much faster parsing in browsers when compared to JS or asm.js) - https://hacks.mozilla.org/2018/10/calls-between-javascript-and-webassembly-are-finally-fast-%F0%9F%8E%89/
* Making web ecosystem inclusive - https://github.com/appcypher/awesome-wasm-langs
* A great browser support - https://caniuse.com/#feat=wasm.
* Improving day by day! - https://github.com/WebAssembly/proposals

## Keywords related to WebAssembly
### asmjs
* Mozilla's experimental technology, first attempt to include other languages to the web!
* asm.js is a subset of JavaScript designed to allow computer software written in languages such as C to be run as web applications.
* asm.js can be bundled inside the main JS file, while as mentioned earlier WebAssembly is a binary file on the side, so you will have more than one file to distribute.
* For older browsers where WASM is not supported yet, WASM can be compiled into asm.js by JavaScript polyfill.

### emscripten: 
- An Open Source LLVM to JavaScript compiler.
- A toolchain for compiling to asm.js and WebAssembly. 
- Built using LLVM
- Lets you run C and C++ on the web at near-native speed without plugins.
- Compiles to WebAssembly by default, but you can also compile to JS for older browsers.
- C/C++/..   ==>>  LLVM  ==>>  [Emscripten]  ==>>  JS

### LLMV
- The LLVM Project is a collection of modular and reusable compiler and toolchain technologies. Despite its name, LLVM has little to do with traditional virtual machines. The name "LLVM" itself is not an acronym; it is the full name of the project.
- LLVM is a library that is used to construct, optimize and produce intermediate and/or binary machine code.
- LLVM can be used as a compiler framework, where you provide the "front end" (parser and lexer) and the "back end" (code that converts LLVM's representation to actual machine code).
- LLVM can also act as a JIT compiler - it has support for x86/x86_64 and PPC/PPC64 assembly generation with fast code optimizations aimed for compilation speed.

## Interesting articles/resources:
* https://developer.mozilla.org/en-US/docs/WebAssembly/Concepts
* https://webassembly.org/getting-started/js-api/
* https://codelabs.developers.google.com/codelabs/web-assembly-intro/index.html#0
* https://blog.mozilla.org/blog/2017/03/07/lots-new-in-firefox-game-changing-webassembly-support/
* https://www.webassemblyman.com/webassembly_front_end_web_development.html
* https://kripken.github.io/talks/wasm.html#/

## Evangelism:
https://github.com/gurumukhi/webassembly-cheatsheet/tree/master/evangelism
