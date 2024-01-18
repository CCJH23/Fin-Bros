# FINBROS LETS GO

## Website UI
![Home Page](https://github.com/CCJH23/Fin-Bros/blob/be0995f8a55ce4e9928261d36c6c2db35ee0bf6f/homepage2.png)

## Start frontend app:

- ```cd frontend```
- ```npm i```
- ```npm run dev```
- IF you encounter a styled_prop error, delete frontend/node_modules and package-lock.json, and ```npm install``` again

## Backend Application:

Backend Application can be connected locally or to a cloud hosted ec2.
The cloud hosted ec2 has redis installed on the stocks collection in MongoDB to ease data retrieval rate.

## Common backend error:

- If error, try reloading project on pom.xml.
- If env files are missing, go to:
- contact @ryanpoy on telegram for files

## Connecting to springboot hosted on cloud (ec2):

- In the frontend/src/stores/AppStore.tsx, comment out line 6.
- Uncomment line 9

## Start Backend App (Running through VSCODE):

- Install Extension Pack for Java
- click on run code

## Start Backend App (through terminal) with Maven installed (Windows):

- ```mvn clean install```
- ```cd backend```
- ```create target/classes```
- ```compile.bat```
- ```run.bat```
<!-- - mvn clean install && mvn spring-boot:run -->

## Start Backend App (through terminal) with Maven installed (Mac):

- ```cd backend```
- ```mvn clean install```
- ```mkdir target/classes```
- ```bash "./compile.sh"```
- ```bash "./run.sh"```

## For FinBros Developers

## Guidelines:

- write all components and views in .tsx
- write any reusable functions in .js
- use Pascal casing HelloWorld.tsx

## SPA

- App.tsx is main app file
- main.tsx is the single page HTML file

## Where to find stuff:

- Assets:
  - css
  - img (any image/svg files)
- components (any reusable components, make sure it's placed in a generic folder):
  - buttons
  - cards
  - forms
- constants (any reusable Constants)
- routes (all routing stuff)
- views (actual screen, also ensure it's placed in generic folder):
  - Login
    - Login.tsx
- stores (state management stuff)

# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
   parserOptions: {
    ecmaVersion: 'latest',
    sourceType: 'module',
    project: ['./tsconfig.json', './tsconfig.node.json'],
    tsconfigRootDir: __dirname,
   },
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list
