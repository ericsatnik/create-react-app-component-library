[View README.md](../README.md)

This template was bootstrapped with [create-react-app](https://github.com/facebook/create-react-app) and [storybook](https://github.com/storybookjs/storybook)


# Build this template from scratch

## Step 1: Create A New Project

Create a new `create-react-app` project, name it create-react-app-component-library, and install packages

```
 npx create-react-app create-react-component-library
```

## Step 2: Add Storybook 

```
npx -p @storybook/cli sb init
```

## Step 3: Install dependencies

```
npm install concurrently polished react-spring styled-components styled-components-modifiers --save
```

Learn more about these packages: 

- [concurrently](https://github.com/kimmobrunfeldt/concurrently)
- [polished](https://github.com/styled-components/polished)
- [react-spring](https://github.com/react-spring/react-spring)
- [styled-components](https://github.com/styled-components/styled-components)
- [styled-components-modifiers](https://github.com/Decisiv/styled-components-modifiers)


## Step 4: 

Install dev dependencies

```
npm install @storybook/addon-a11y @storybook/addon-backgrounds @storybook/addon-contexts @storybook/addon-docs @storybook/addon-knobs --save-dev
```
 Learn more about these packages:

- [storybook/addons/a11y](https://github.com/storybookjs/storybook/tree/master/addons/a11y)
- [storybook/addons/backgrounds](https://github.com/storybookjs/storybook/tree/next/addons/backgrounds)
- [storybook/addons/contexts](https://github.com/storybookjs/storybook/tree/master/addons/contexts)
- [storybook/addons/docs](https://github.com/storybookjs/storybook/tree/master/addons/docs)
- [storybook/addons/knobs](https://github.com/storybookjs/storybook/tree/master/addons/knobs)


## Step 4: Update `scripts` in `package.json`

```
    "start": "concurrently \"npm run client\" \"npm run storybook\"",
    "client": "react-scripts start",
    "build": "concurrently \"react-scripts build\" \"build-storybook\"",
    "test": "react-scripts test",
    "eject": "react-scripts eject",
    "storybook": "start-storybook -p 9009 -s public",
    "build-storybook": "build-storybook -s public"
```

## Step 5: Start `create-react-app-component-library` 

```
npm run start
```

Runs the app in the development mode.

Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

Runs storybook in development mode

Open [http://localhost:9090](http://localhost:9090) to view it in the browser.