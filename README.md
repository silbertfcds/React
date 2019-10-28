## Tecnologias

- Node
- Npm
- Yarn

Instalando o pacote do react:

### `npm install -g create-react-app`

Agora com o pacote do react instalado, só executar o comando?

### `create-react-app NOMEPROJETO`

Instalando o pacote do axios para requisição ajax:

### `yarn add axios`

Instalando o pacote de criação de rotas:

### `yarn add react-router-dom`

Adicionar o arquivo **_.editorconfig_** usando o plugin do Vs code chamado **EditorConfig for VS Code**. Para criar o arquivo basta clicar botão direito do mouse e escolher a opção **generate .editorconfig**.

Configurando do zero ESlint, apagar no arquivo package.json a configuração:

    "eslintConfig": {
        "extends": "react-app"
    }

Instalando o pacote do eslint como dependência de desenvolvimento:

### `yarn add eslint -D`

Agora vamos configurar o eslint no projeto, primeiro vamos digitar:

### `yarn eslint --init`

Agora vão aparecer opções para serem escolhidas. Vamos escolher:

1. To check syntax, find problems, and enforce code style
2. JavaScript modules (import/export)
3. React
4. Browser
5. Use a popular style guide
6. Airbnb
7. Javascript

Para atualizar as dependências do projeto é necessário apagar o arquivo **_package-lock.json_** e rodar o comando:

### `yarn`

Instalar o pacote do prettier com o eslint:

### `yarn add prettier eslint-config-prettier eslint-plugin-prettier babel-eslint -D`

Vamos configurar o arquivo **_.eslinttrc.js_** no projeto:

    module.exports = {
        env: {
            browser: true,
            es6: true,
        },
        extends: [
            'airbnb',
            'prettier',
            'prettier/react'
        ],
        globals: {
            Atomics: 'readonly',
            SharedArrayBuffer: 'readonly',
        },
        parser: 'babel-eslint',
        parserOptions: {
            ecmaFeatures: {
            jsx: true,
            },
            ecmaVersion: 2018,
            sourceType: 'module',
        },
        plugins: [
            'react',
            'prettier'
        ],
        rules: {
            'prettier/prettier': 'error',
            'react/jsx-filename-extension': [
                'warn',
                { extensions: ['.jsx', '.js'] }
            ],
            'import/prefer-default-export': 'off'
        },
    };

Vamos criar o arquivo **_.prettierrc_**

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br>
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br>
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (Webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `npm run build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify
