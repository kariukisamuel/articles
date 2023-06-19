---
title: "A Short Introduction To How TypeScript Made Javascript Cool."
datePublished: Mon Jun 19 2023 09:34:44 GMT+0000 (Coordinated Universal Time)
cuid: clj2nu8df000609jxdpt9fybd
slug: a-short-introduction-to-how-typescript-made-javascript-cool
canonical: https://dev.to/bazeng/a-short-introduction-to-how-typescript-made-javascript-cool-5a9o
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1687167136237/d667f9c3-0495-4e5a-88c7-ed889704f30e.png
tags: javascript, react-native, nodejs, reactjs, typescript

---

Yes, you've read the headline correctly! If you're currently perusing this article, chances are you've noticed the increasing demand for TypeScript as a preferred skill in modern JavaScript job advertisements. There's a clear rationale behind this preference. In a series of articles, I will delve into TypeScript, covering topics ranging from the fundamentals to more advanced concepts. My goal is to provide guidance that will transform you from a TypeScript novice into a proficient developer.

## Why Typescript?

Before we can understand what TypeScript is, it's important to understand why it was created and what problem it solves. When JavaScript was first created, its inventors never imagined that it would be used in the large and complex applications that we see today. JavaScript was originally a simple scripting language that was used to add dynamic behavior to static web pages. However, over time, JavaScript has evolved to be used to create rich, interactive web applications that are connected to web APIs. It has even evolved to be used outside of the browser, on servers, using Node.js.

## What sets Typescript apart from Javascript?

If you are familiar with how JavaScript code is executed, you know that it is a two-step process: **parsing and execution**. However, TypeScript adds an additional step before parsing, which is **type checking and transpilation(converting typescript to javascript)**.

Please refer to the diagram below for a visual representation of the differences in execution between JavaScript and TypeScript:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1687166146371/15a3daba-f2fc-470b-9a62-57f667d8b830.png align="center")

## What is Typescript?

In lay man terms **Typescript** is a programming language built on top of JavaScript that brings new features like ***static typing, interfaces & generics.*** It can also be seen as a helpful tool for JavaScript development.

## Where is Typescript Used?

JavaScript is specifically designed to run within dedicated runtime environments like web browsers or Node.js. On the other hand, TypeScript cannot be directly executed within JavaScript runtime environments; instead, it runs within a developer's integrated development environment (IDE).

## What advantages does TypeScript offer compared to plain JavaScript?

Prior to TypeScript's introduction, identifying and resolving type inconsistencies in JavaScript necessitated the manual process of writing and executing code, which could be tiresome. However, TypeScript revolutionized this by offering built-in mechanisms that proactively detect type inconsistencies while coding. It provides features such as autocompletion, code navigation, and refactoring tools, enhancing productivity and streamlining the development experience. These capabilities not only improve efficiency but also provide convenience when writing code

## Now, let's explore some practical use cases:

So Let's say we have a function named **"add"** that requires two arguments, **"a"** and **"b,"** which must both be **numbers**. This function returns the result of adding "a" and "b" together. In JavaScript, the code would look like this:

```javascript
add = (a, b) ->
  return a + b
```

To display the sum of two numbers, such as 10 and 5, we would use the following code:

```javascript
add(10, 5)
```

The expected result would be 15. However, let's consider what would happen if we were to call the function like this:

```javascript
add(10, "5")
```

Can you guess the outcome? The result would be **"105."** Typescript serves the purpose of preventing us from falling into such pitfalls. Nonetheless, if we were to utilize Typescript, our code would appear as follows in the IDE:

```javascript
const add = (a: number, b: number): number => {
  return a + b;
};
```

If you find it challenging to comprehend the code mentioned above, don't worry. We will explore it in more detail later on. Continuing with the previous example, if we were to invoke the "add" function like this:

```javascript
add(10, "5")
```

Even before running this function, TypeScript would warn us with an error stating:

Argument of type 'string' is not assignable to parameter of type 'number'

This error holds significant importance as it ensures the integrity of our code by preventing incompatible types from being used.

## Installing TypeScript: A Step-by-Step Guide

Here is a step-by-step guide on how to utilize TypeScript:

**1\. Installation:**

To install TypeScript, you have three options depending on your usage requirements:

> **a) npm module installation:**

> ```javascript
> npm install typescript --save-dev
> ```
> 
> **b) NuGet package:**

> There are two methods to install TypeScript via Visual Studio:

* Use the "Manage NuGet Packages" window by right-clicking on a project node.
    
* Access the NuGet Package Manager Console under Tools &gt; NuGet Package Manager &gt; Package Manager Console. Use the command `Install-Package Microsoft.TypeScript.MSBuild.`
    

> **c) As a Visual Studio Extension:** If your project type does not support NuGet, you can utilize the TypeScript Visual Studio extension. To install the extension, navigate to Extensions &gt; Manage Extensions in Visual Studio.

## Setting up a TypeScript Project: Step-by-Step Instructions

1. Create a new directory for your TypeScript project and navigate to it using the command line.
    
2. Run the command: `tsc --init` to generate a **tsconfig.json** file, which will contain your TypeScript project's configuration options. When a directory contains a tsconfig.json file, it signifies that the directory serves as the main location for a TypeScript project. The tsconfig.json file defines the root files and compiler options necessary for compiling the project.
    
3. Start writing your TypeScript code in `.ts` files using the TypeScript language syntax. Take advantage of TypeScript's additional features such as static typing, interfaces, classes, and modules to enhance your code.
    
4. Compiling TypeScript Code: After writing your TypeScript code, compile it into JavaScript. Use the tsc command to invoke the TypeScript compiler. By default, the compiler will look for the `tsconfig.json` file in the current directory and generate the corresponding JavaScript files.
    
5. Execute the generated JavaScript code using a JavaScript runtime environment or a web browser. You can include the compiled JavaScript files in your HTML files or run them through a Node.js environment, depending on your project's requirements.
    
6. Make changes to your TypeScript code, recompile it, and rerun the JavaScript code as needed. TypeScript's type-checking and compiler feedback will assist you in catching errors and improving the codebase.
    

**Note:** When it comes to JavaScript frameworks like React, Vue or Node.js, TypeScript is often bundled within their installation process. This integration allows you the freedom to choose whether or not to leverage TypeScript in your project, providing flexibility based on your specific needs and preferences.

## How JavaScript was made cool by TypeScript:

1. **Real-time Type Error Detection:** Type errors are alerted by TypeScript as code is written, eliminating the need for compilation to discover errors. This feature saves time for developers and simplifies the process of writing code.
    
2. **Time-saving Development:** Type errors are identified during development by TypeScript, enabling developers to catch and resolve issues early on, reducing the time spent on debugging and troubleshooting.
    
3. **Enhanced Code Writing Experience:** The coding experience is improved by TypeScript through the provision of features such as autocompletion, code navigation, and refactoring tools. These features contribute to enhanced productivity and make the process of writing code more convenient