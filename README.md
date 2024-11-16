<<<<<<< HEAD
# Telegram Mini App + Dynamic connect

Steps to have the Telegram Mini App (TMA) + Bot running

1. Create a Bot on Telegram using Botfather, [link to tutorial](https://core.telegram.org/bots/tutorial#getting-ready)
2. Clone this repo, run `cp .env.sample .env` and use your own Dynamic environment ID by replacing `NEXT_PUBLIC_DYNAMIC_ENV_ID` in the `.env` file
3. Deploy your website online. [link to tutorial](https://vercel.com/docs/deployments/git#deploying-a-git-repository)
4. Using Botfather, add the website url that should be opened for your TMA. [link to tutorial](https://docs.ton.org/develop/dapps/telegram-apps/step-by-step-guide#3-set-up-bot-mini-app)
5. Use Bot `TOKEN` from Telegram and your website url as LOGIN_URL in the `.env` file.
6. Run telegram bot `ts-node scripts/bot.ts`. If you do not have `ts-node` you can install it by running `npm -g i ts-node`
7. Go to your Telegram Bot and type `/start`

[Build Around the Booming Telegram Ecosystem](https://www.dynamic.xyz/ecosystems/telegram)
=======
# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
export default tseslint.config({
  languageOptions: {
    // other options...
    parserOptions: {
      project: ['./tsconfig.node.json', './tsconfig.app.json'],
      tsconfigRootDir: import.meta.dirname,
    },
  },
})
```

- Replace `tseslint.configs.recommended` to `tseslint.configs.recommendedTypeChecked` or `tseslint.configs.strictTypeChecked`
- Optionally add `...tseslint.configs.stylisticTypeChecked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and update the config:

```js
// eslint.config.js
import react from 'eslint-plugin-react'

export default tseslint.config({
  // Set the react version
  settings: { react: { version: '18.3' } },
  plugins: {
    // Add the react plugin
    react,
  },
  rules: {
    // other rules...
    // Enable its recommended rules
    ...react.configs.recommended.rules,
    ...react.configs['jsx-runtime'].rules,
  },
})
```
>>>>>>> 0ee14318b4ec78c8021529090042a6d983873b35
