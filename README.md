# Astro Starter Kit

```
npm create astro-starter@latest
```

[![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/zankhq/astro-starter)
[![Open with CodeSandbox](https://assets.codesandbox.io/github/button-edit-lime.svg)](https://codesandbox.io/p/sandbox/github/zankhq/astro-starter)
[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/zankhq/astro-starter?devcontainer_path=.devcontainer/blog/devcontainer.json)

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

![blog](https://github.com/withastro/astro/assets/2244813/ff10799f-a816-4703-b967-c78997e8323d)

Features:

- ✅ Tailwind CSS
- ✅ Alpine js
- ✅ Dark/light mode
- ✅ Blog
- ✅ Discussions (thanks to giscus)
- ✅ CMS for editing blog post (thanks to decap CMS)
- ❌ PWA

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```
├── public/
├── src/
│   ├── components/
│   ├── content/
│   ├── layouts/
│   ├── locales/
│   ├── middleware/
│   ├── pages/
│   ├── styles/
│   ├── utils/
│   └── consts.ts/
├── astro.config.mjs
├── README.md
├── package.json
├── .prettierrc
├── tailwind.config.cjs
└── tsconfig.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

The `src/content/` directory contains "collections" of related Markdown and MDX documents. Use `getCollection()` to retrieve posts from `src/content/blog/`, and type-check your frontmatter using an optional schema. See [Astro's Content Collections docs](https://docs.astro.build/en/guides/content-collections/) to learn more.

Any static assets, like images, can be placed in the `public/` directory.

## ✍️ Admin dashboard

You can access the admin dashboard for editing blog post at `/admin` (https://example.com/admin)

For more information follow Decap CMS documentation at https://decapcms.org/docs/

In order to access the admin dashboard to change blog articles content you need to have access to the github repo, a quick way to test it test would be fork the repo and than configure decap cms accordingly to your cloud provider (netlify, cloudflare, vercel, etc...).

If you use cloudflare pages you can follow this guide https://github.com/i40west/netlify-cms-cloudflare-pages.

In this case your environment variable should look like this

![Cloudflare environment variable image](.github/images/cloudflare-env-var.png)

If you use netlify it's actually easier, you will need to change in the file `astro.config.mjs` NetlifyCMS config `config.backend.name` to git-gateway. (See https://decapcms.org/docs/git-gateway-backend/#git-gateway-with-netlify for more info)

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Check out [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).

## Credit

This theme is based off of the lovely [Bear Blog](https://github.com/HermanMartinus/bearblog/).
