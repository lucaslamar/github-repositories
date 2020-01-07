<h1 align="center">GitHub Users</h1>



</h3>
<p align="center">
  <b>Github Users</b> é uma simples single page que usa api to Github para fazer a listagem de Repostitorios e mostrar os detalhes do mesmo, vale lembra que o projeto utiliza ' . <br>  styled-components 💅</p>

![demo](../assets/demo.png)

### Support
- [Become a backer or sponsor on Patreon](https://www.patreon.com/arturbien).
- [One-time donation via PayPal](https://www.paypal.me/react95)


## Getting Started
First, install component library and styled-components in your project directory:
```sh
$ npm i react95 styled-components
```
Apply style reset, wrap your app content with ThemeProvider with theme of your choice... and you are ready to go! 🚀
```jsx
import React from "react";
import { createGlobalStyle, ThemeProvider } from "styled-components";
import { reset, themes, List, ListItem, Divider } from "react95";

const ResetStyles = createGlobalStyle`
  ${reset}
`;

export default props =>
  <div className="App">
    <ResetStyles />
    <ThemeProvider theme={themes.default}>
      <List>
          <ListItem>🎤 Sing</ListItem>
          <ListItem>💃🏻 Dance</ListItem>
          <Divider />
          <ListItem disabled>😴 Sleep</ListItem>
      </List>
    </ThemeProvider>
  </div>

```

### Explore
You can view components on [Storybook](https://arturbien.github.io/React95/). If you want to play with it locally, simply clone the repo and run commands below:
```sh
$ npm i
$ npm run storybook
```
### Submit your project
Apps built with React95 will be submitted on the official React95 [website](https://react95.io) 🤟🏻

### Contributing
**We are not attempting to exactly RECREATE Windows95 components. We are going to make them usable in the modern mobile / web apps.
Thus, any help from UI / UX designers would be EXTREMELY appreciated. The challenge is to come up with new component designs / layouts that are broadly used in modern UIs, that weren't present back in 95.**

There's a lot to do. If you want to help with the project, feel free to open pull requests and submit issues. Let's make UI great again 🔥

### Roadmap
There's quite a few things to be done:
- Styled system
- Lots of tacky color schemes 🌈
- Custom icons maybe? (Emojis from Windows 10 seem to go very well with the lib)
- Typography
- Range slider component
- Avatar component
- Components common in all modern UIs (FAB, Badge, Avatar, Snackbar, Steppers)

And the boring stuff too:
- Testing
- Semantic release
- eslint
