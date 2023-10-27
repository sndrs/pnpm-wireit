# pnpm/wireit PoC

> Example monorepo that uses [pnpm](https://pnpm.io) to manage packages and orchestrate tasks, [wireit](https://github.com/google/wireit) to handle output caching and follows GitHub's [Scripts to Rule Them All](https://github.blog/2015-06-30-scripts-to-rule-them-all/).
>
> It's an exploration of a closer-to-the-metal alternative to Nx, Turborepo et al.

## How to use it

1. Clone the repo
2. Run `./scripts/build`.

That will install dependencies and build all projects.

To build specific projects, run:

```sh
./scripts/build <package-name>
```

For example, to build the example vite app in `apps/vite-react-app`, including all its internal dependencies, run:

```
./scripts/build "vite-react-app"
```

To build all `@guardian` packages (also including all internal dependencies), run:

```sh
./scripts/build "@guardian/*"
```
