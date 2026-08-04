# my-app

An [Astro](https://astro.build) & [Void](https://void.cloud) wired starter project.

## Getting Started

This project requires [pnpm](https://pnpm.io) 11.x and Node.js >=24.

```sh
git clone https://github.com/derrickobedgiu1/void-astro-starter my-app
cd my-app
pnpm install
pnpm dev
```

The dev server starts at `localhost:4321`.

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
├── src/
│   └── pages/
│       └── index.astro
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                | Action                                           |
| :--------------------- | :----------------------------------------------- |
| `pnpm install`         | Installs dependencies                            |
| `pnpm dev`             | Starts local dev server at `localhost:4321`      |
| `pnpm build`           | Build your production site to `./dist/`          |
| `pnpm preview`         | Preview your build locally, before deploying     |
| `pnpm astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `pnpm astro -- --help` | Get help using the Astro CLI                     |

## 🚀 Deploy

This project uses the `@astrojs/cloudflare` adapter, so it deploys to your Cloudflare account via Wrangler rather than `void deploy --backend cloudflare` (currently doesn't yet support framework SSR).

```sh
pnpm run deploy
```

First deploy provisions any missing bindings (e.g. the `SESSION` KV namespace) automatically and writes their IDs back to `wrangler.jsonc`.

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).
