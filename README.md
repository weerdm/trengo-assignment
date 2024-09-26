# Trengo - Frontend Interview Assignment

This template should help get you started developing with Vue 3 with Vite. It contains nothing more than the basic skeleton with which you can start developing the solution to the given assignment. You may modify it if you so wish, but it's not necessary. Tailwind has already been pre-configured for you. Should you wish to add any more packages for whatever reason, feel free to do so.

Should you have any issues running this, please reach out to us ASAP and we'll help you through it.

## Project Setup

First, pull this repository to your machine, and run the below command:

```sh
npm install
```

This will install all the project's dependencies for you.

**IMPORTANT**: You should also delete the `.git` folder & re-initialize the repo once you've run `npm install`. This will allow you to start with a clean `git` history.

You can do so by running the following commands (Make sure that you're inside the repo when you run these, as they are destructive and involve deletion of git history)

```sh
# Deletes the .git folder and everything in it
rm -rf ./.git

# Re-initializes the repository
git init

# Adds all the current files as they are as the first commit
git add . && git commit -m "Initialize interview assignment"
```

You will now have a fresh history, and can start making changes to the project. Once you're done, make sure to upload your solution to Github under your own account in a private repository, and make sure to give your contact person (It'll be in the assignment document you received) permission to view the repository.

## Type Support for `.vue` Imports in TS

TypeScript cannot handle type information for `.vue` imports by default, so we replace the `tsc` CLI with `vue-tsc` for type checking. In editors, we need [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) to make the TypeScript language service aware of `.vue` types.

### Compile and Hot-Reload for Development

```sh
npm run dev
```

### Type-Check, Compile and Minify for Production

```sh
npm run build
```

### Run Unit Tests with [Vitest](https://vitest.dev/)

```sh
npm run test:unit
```

### Run End-to-End Tests with [Playwright](https://playwright.dev)

```sh
# Install browsers for the first run
npx playwright install

# When testing on CI, must build the project first
npm run build

# Runs the end-to-end tests
npm run test:e2e
# Runs the tests only on Chromium
npm run test:e2e -- --project=chromium
# Runs the tests of a specific file
npm run test:e2e -- tests/example.spec.ts
# Runs the tests in debug mode
npm run test:e2e -- --debug
```

### Lint with [ESLint](https://eslint.org/)

```sh
npm run lint
```
