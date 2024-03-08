# INTRODUCTION

- [INTRODUCTION](#introduction)
  - [What is JavaScript](#what-is-javascript)
  - [Why was JS created?](#why-was-js-created)
  - [How is JavaScript executed?](#how-is-javascript-executed)
  - [Execution Contexts](#execution-contexts)
    - [Global Execution Context (GEC)](#global-execution-context-gec)
    - [Function Execution Context (FEC)](#function-execution-context-fec)
      - [Call stack](#call-stack)
      - [Creation Phase](#creation-phase)
      - [Execution Phase](#execution-phase)
  - [Setting up a development environment](#setting-up-a-development-environment)

## What is JavaScript

JavaScript is a dynamic, weakly typed programming language which is compiled at runtime. It can be executed as part of a webpage in a browser or directly on any machine ("host environment"). It is commonly refered to as JS.

JavaScript was created to make webpages more dynamic (e.g change content on a page directly from inside the browser). Originally, it was called LiveScript but due to the popularity of Java, it was named JavaScript. Although it's name is inherited from Java, when it comes to how the language is structured and written, JS is completely independent and has mostly nothing to do with Java.

## Why was JS created?

The main reason for creating JS was to five web developers a way to add more engaging elements to websites, rather that static content. With JS, web pages could respond to user input and create a more dynamic user experience. In order to understand how JS can make pages more responsive, a basic understanding of how navigating the web works.

When a user visits and interacts with a client (browser). More precisely, when a webpage is visited, a request is sent to a server where the html file is hosted, this server than processes that request and produces a response, the most simple type of response is a HTML page that is sent to the user/client. This is done for every request done within the page. JavaScript comes in to increase the website's responsiveness, making it more dynamic overall.

## How is JavaScript executed?

JavaScript execution relies on two main concepts, execution contexts and the call stack, and two main phases, creation phase and execution phase. This process ensures that JS code is executed in a structured and predictable manner.

## Execution Contexts

These are special environments created by the JavaScript engine to manage code execution. There are two types:

### Global Execution Context (GEC)

Created first, it holds all globally defined variables and functions.

### Function Execution Context (FEC)

Created for each function call, it manages function-specific variables, arguments, and the code itself.

#### Call stack

This is a data structure (often visualized as a stack of plates) that keeps track of the order in which functions are called. It follows LIFO, last-in-first-out principle. When the script starts, the GEC is created and pushed onto the call stack. When a function is called, a new FEC is created, pushed onto the stack, and its code is executed. Once the function finishes, its FEC is popped off the stack, and execution resumes in the previous context.

#### Creation Phase

The engine parses the code, allocates memory for variables, and sets up the scope chain (how the context finds variables).

#### Execution Phase

The engine goes line by line, executing statements and expressions. Function calls create new contexts and push them onto the stack.

## Setting up a development environment

To develop, not only JS, but any programming language, it's a good idea to use a code editor. This is obviously not required, given that there are many many ways of writing files and running them, some of them from within the OS not needing to install anything whatsoever, like the noteblock in windows, or vim in macOS and Linux.

A good recomendation is using VsCode as a code editor. This is a very modern and fast IDE (Integrated Development Environment), it can be combined with a lot of extensions that can be installed from within the IDE. To develop JS, its also important to have an environment where the webpage / code can be tested, more specifically a browser, be it edge, opera, google chrome.

VsCode can be downloaded with this [link](https://code.visualstudio.com/download), same for Chrome with this [link](https://www.google.com/chrome/dr/download/).