# cra-template-wdever

![Publish](https://github.com/WDever/cra-template-wdever/workflows/Publish/badge.svg?event=release)

Template for my side projects.

[EXAMPLE](https://github.com/WDever/redux-toolkit-example)

## Modules
- default CRA Typescript modules
- redux
- redux-saga
- redux-toolkit
- axios
- moment
- query-string
- polyfill
- react-router-dom
- styled-components

## Config
- ESLint with airbnb rule and Typescript
- Prettier

## Architecture
- public : CRA's default public dir
- src
  - assets : Some assets like fonts / images
  - components : All of your components. but NO ROUTE
  - hooks : Custom hooks that access to redux store or dispatch actions
  - pages : Just route your pages. combine components.
  - store : Write redux code. Ducks pattern or separate each files? It's your choice
    - (example of separating each files) action
    - model
    - reducer
    - saga
  - utils : A collection of useful things like functions, custom hooks, utility styles, utility types
  - App.tsx : Combine all your pages and route them
  - root.tsx : Base settings for redux, react-router-dom, global style
- .env : Cutom enviroment var
- .prettierrc: Prettier configuration
- .eslintrc.json : ESLint configuration 

## Usage
To use this template, add `--template wdever` when creating a new app.

For example:

```sh
npx create-react-app my-app --template wdever

# or

yarn create react-app my-app --template wdever
```
