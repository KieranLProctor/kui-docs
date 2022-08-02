---
sidebar_position: 1
---

# Getting Started

Let's discover everything that **[@kieranlproctor/kui](https://github.com/KieranLProctor/kui)** has to offer.

### What you'll need

- [Node.js](https://nodejs.org/en/download/) version 16.14 or above:
  - When installing Node.js, you are recommended to check all checkboxes related to dependencies.
- [ReactJS](https://reactjs.org) app created.
- [Tailwind CSS](https://tailwindcss.com) added to the app.

## Adding Kui

To add **[@kieranlproctor/kui](https://github.com/KieranLProctor/kui)** simply run one of these commands:

```bash
npm install @kieranlproctor/kui
```
// or
```bash
yarn add @kieranlproctor/kui
```

You can type this command into Command Prompt, Powershell, Terminal, or any other integrated terminal of your code editor.

The command also installs all necessary dependencies you need to use **[@kieranlproctor/kui](https://github.com/KieranLProctor/kui)**.

## Tailwind CSS Configurations

Once you install **[@kieranlproctor/kui](https://github.com/KieranLProctor/kui)** you need to wrap your tailwind css configurations with the `withConfig()` function coming from **[@kieranlproctor/kui/utils](https://github.com/KieranLProctor/kui/utils)**.

```js {1, 3, 9}
// This was added
const withMT = require("@kieranlproctor/kui/utils/withConfig");

// This was added
module.exports = withMT({
  content: ["./pages/**/*.{js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
// This was added
});
```
