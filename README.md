# Vitesse theme for Astro

Vitesse theme for Astro blog, supports Vue and UnoCSS.

[![Netlify Status](https://api.netlify.com/api/v1/badges/d5bae292-6116-4c52-af4b-05eadedccc60/deploy-status)](https://app.netlify.com/sites/kaivanwong/deploys)

## Preview

![Preview Image](./preview.jpg)

## Quick Start

[![Deploy to Netlify Button](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/kaivanwong/astro-theme-vitesse)

Click this button, it will create a new repo for you that looks exactly like this one, and sets that repo up immediately for deployment on Netlify.

If you  just want to develop locally, you can [create a repo](https://github.com/kaivanwong/astro-theme-vitesse/generate) from this template on GitHub.

## Usage

Just run and visit http://localhost:1977.

```bash
npn run dev
```

> Node.js version 18 or higher is required for this project.

To build the App, you can run:

```bash
npm run build
```

You will then see the `dist` folder generated for publishing, which you can preview locally with the following command.

```bash
npm run preview
```

## Use pnpm / yarn

If you want to use pnpm or yarn as a package management tool, please refer to the following steps.

> If `preinstall` exists in `scripts`, remove it first.

### pnpm

Replace `"pre-commit": "npx lint-staged"` in package.json with `"pre-commit": "pnpm lint-staged"`.

And replace `"*": "npm run lint:fix"` with `"*": "pnpm lint:fix"`.

Like this:

```json
{
  // ...
  "simple-git-hooks": {
    "pre-commit": "pnpm lint-staged"
  },
  "lint-staged": {
    "*": "pnpm lint:fix"
  }
}
```

### yarn

Replace `"pre-commit": "npx lint-staged"` in package.json with `"pre-commit": "yarn lint-staged"`.

And replace `"*": "npm run lint:fix"` with `"*": "yarn lint:fix"`.

Like this:

```json
{
  // ...
  "simple-git-hooks": {
    "pre-commit": "yarn lint-staged"
  },
  "lint-staged": {
    "*": "yarn lint:fix"
  }
}
```

## License

[MIT License](./LICENSE) © 2024-PRESENT [Kaivan Wong](https://github.com/kaivanwong)
