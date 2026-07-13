# Portfolio OS

My personal portfolio website built as a simulated desktop operating system, which includes windows, a dock, a terminal, and apps. Built with React, TypeScript, Vite, and Tailwind CSS.

## Prerequisites

- **Node.js 24** (pinned in `.nvmrc`)
  - Using [mise](https://mise.jdx.dev): run `mise settings add idiomatic_version_file_enable_tools node` once, then `mise install` in this directory
  - Using [nvm](https://github.com/nvm-sh/nvm): `nvm use`
- **npm 10+** (ships with Node 24)

Node/npm versions below the pinned minimums are rejected automatically (`.npmrc` sets `engine-strict=true`).

## Getting started

```bash
git clone https://github.com/adriankristanto/portfolio-os.git
cd portfolio-os
npm install
npm run dev
```

The dev server starts at `http://localhost:5173`.

## Scripts

| Script         | Command                                                     | Purpose                             |
| -------------- | ----------------------------------------------------------- | ----------------------------------- |
| `dev`          | `vite`                                                      | Start the local dev server          |
| `build`        | `tsc -b && vite build`                                      | Production build to `dist/`         |
| `preview`      | `vite preview`                                              | Serve the production build locally  |
| `lint`         | `eslint .`                                                  | Run ESLint on the project           |
| `format`       | `prettier --write .`                                        | Format code with Prettier           |
| `format:check` | `prettier --check .`                                        | Check code formatting with Prettier |
| `typecheck`    | `tsc --noEmit`                                              | Type-check the project              |
| `verify`       | `npm run typecheck && npm run lint && npm run format:check` | Run all verification checks         |

More scripts (testing, linting, CI helpers) will be added here as they're introduced.

## License

Code in this repository is licensed under the [MIT License](./LICENSE).

Personal content and branding, including resume text, project write-ups, photos, logo, avatar, and wallpapers, is © Adrian Kristanto, all rights reserved, and is **not** covered by the MIT license.
