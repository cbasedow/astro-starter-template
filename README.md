# Astro Starter Template

Reusable starter for Astro projects with Tailwind CSS v4, ESLint, Prettier, and TypeScript preconfigured.

## Stack

- [Astro](https://astro.build/) 6
- [Tailwind CSS](https://tailwindcss.com/) v4 via `@tailwindcss/vite`
- [Prettier](https://prettier.io/) with `prettier-plugin-astro` and `prettier-plugin-tailwindcss`
- [ESLint](https://eslint.org/) flat config with `eslint-plugin-astro`, `typescript-eslint`, `eslint-plugin-jsx-a11y`, and `eslint-plugin-simple-import-sort`
- [TypeScript](https://www.typescriptlang.org/) strict mode with type checking via `@astrojs/check`

## Start a new project

Requires [Node.js](https://nodejs.org/) 22.12+ and [pnpm](https://pnpm.io/).

### From GitHub (recommended)

Requires the [GitHub CLI](https://cli.github.com/) (`gh`).

Create a new repo from this template and clone it in one step:

```sh
gh repo create my-new-site --template cbasedow/astro-starter-template --public --clone
cd my-new-site
pnpm install
pnpm dev
```

Update `name` in `package.json`.

If you already created the repo with **Use this template** on GitHub:

```sh
gh repo clone cbasedow/<your-new-repo>
cd <your-new-repo>
pnpm install
pnpm dev
```

### Without GitHub CLI

Clone this template directly, then reset git history if you want a fresh start:

```sh
git clone https://github.com/cbasedow/astro-starter-template.git my-new-site
cd my-new-site
rm -rf .git && git init
pnpm install
pnpm dev
```

## Commands

| Command             | Action                                |
| :------------------ | :------------------------------------ |
| `pnpm install`      | Install dependencies                  |
| `pnpm dev`          | Start dev server at `localhost:4321`  |
| `pnpm build`        | Build for production to `./dist/`     |
| `pnpm preview`      | Preview the production build locally  |
| `pnpm lint`         | Run ESLint                            |
| `pnpm lint:fix`     | Run ESLint with auto-fix              |
| `pnpm format`       | Format with Prettier                  |
| `pnpm format:check` | Check formatting (useful in CI)       |
| `pnpm typecheck`    | Type-check `.astro` and TS files      |
| `pnpm check`        | Run lint, format check, and typecheck |

## Project structure

```text
/
├── public/
├── src/
│   ├── layouts/
│   │   └── BaseLayout.astro
│   ├── pages/
│   │   └── index.astro
│   └── styles/
│       └── global.css
├── .vscode/              # optional editor config (VS Code / Cursor)
├── astro.config.mjs
├── eslint.config.js
├── pnpm-workspace.yaml   # allows native builds (esbuild, sharp); not a monorepo
├── tsconfig.json
└── .prettierrc.json
```

## Editor setup (optional)

The project works without any editor configuration. For VS Code or Cursor, install the recommended extensions when prompted (`.vscode/extensions.json`):

- Astro
- ESLint
- Prettier

Format on save and ESLint autofix are configured in `.vscode/settings.json`.
