# 📦RussianPost calculator API client

[![npm](https://img.shields.io/npm/v/@shevernitskiy/post-calculator?logo=npm&style=flat&labelColor=000)](https://www.npmjs.com/package/@shevernitskiy/post-calculator)
[![JSR](https://jsr.io/badges/@shevernitskiy/post-calculator)](https://jsr.io/@shevernitskiy/post-calculator)
![dependencies](https://img.shields.io/badge/dependencies-0-green?style=flat&labelColor=000)
[![license](https://img.shields.io/github/license/shevernitskiy/post-calculator?style=flat&labelColor=000)](https://github.com/shevernitskiy/post-calculator/blob/main/LICENSE)

This is super simple typed API client for RussianPost Calculator API.
It just fetch calculator response from the API.

# Installation

## Node.js

```sh
npm i @shevernitskiy/post-calculator
```

```sh
npx jsr add @shevernitskiy/post-calculator
```

## Deno

```sh
deno add @shevernitskiy/post-calculator
```

# Usage

Create an instance and call method `tracking`. That's it.

```ts
import { postCalculator } from "@shevernitskiy/post-calculator";

const result = await postCalculator({
  object: 27030,
  from: 115211,
  to: 620000,
  weight: 1000,
});

// result will be typeof PostCalcResponse (typed json)

const result2 = await postCalculator({
  format: "html"
  object: 27030,
  from: 115211,
  to: 620000,
  weight: 1000,
});

// result2 will be typeof string
```

# Contribution

Pull request, issues and feedback are very welcome. Code style is formatted with deno fmt.

# License

Copyright 2024, shevernitskiy. MIT license.
