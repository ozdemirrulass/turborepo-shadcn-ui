# Turborepo Starter Kit: shadcn/ui

This repository features a monorepo architecture for Next.js, preconfigured with shadcn as of October 14, 2024, including the latest versions of the integrated packages. The web application is a Next.js app that utilizes the app router and follows a src directory structure.

![Static Badge](https://img.shields.io/badge/shadcn%2Fui-2.1.0-blue?link=https://github.com/shadcn-ui/ui)
![Static Badge](https://img.shields.io/badge/Next.js-14.2.15-0070f3?link=https://github.com/vercel/next.js)

> [!NOTE]
> This example uses `npm` as package manager.


## Using this Blueprint

Clone the repository:

```sh
git clone https://github.com/ozdemirrulass/turborepo-shadcn-ui.git
```


Install dependencies:

```sh
cd turborepo-shadcn-ui
npm install
```

### Add ui components

Use the pre-made script:

```sh
npm run shadcn <component-name>
```

> This works just like the `shadcn/ui` CLI.

## What's inside?

This Turborepo starter includes the following packages/apps:

- `web`: a [Next.js](https://nextjs.org/) app with src directory and app router.
- `@repo/ui`: a stub React component library (🚀 powered by **shadcn/ui**)
- `@repo/eslint-config`: `eslint` configurations (includes `eslint-config-next` and `eslint-config-prettier`)
- `@repo/typescript-config`: `tsconfig.json`s used throughout the monorepo

Each package/app is 100% [TypeScript](https://www.typescriptlang.org/).

### Build

To build all apps and packages, run the following command:

```sh
cd turborepo-shadcn-ui
turbo build
```

### Develop

To develop all apps and packages, run the following command:

```sh
cd turborepo-shadcn-ui
turbo dev
```

### Remote Caching

Turborepo can use a technique known as [Remote Caching](https://turbo.build/repo/docs/core-concepts/remote-caching) to share cache artifacts across machines, enabling you to share build caches with your team and CI/CD pipelines.

By default, Turborepo will cache locally. To enable Remote Caching you will need an account with Vercel. If you don't have an account you can [create one](https://vercel.com/signup), then enter the following commands:

```
cd turborepo-shadcn-ui
npx turbo login
```

This will authenticate the Turborepo CLI with your [Vercel account](https://vercel.com/docs/concepts/personal-accounts/overview).

Next, you can link your Turborepo to your Remote Cache by running the following command from the root of your Turborepo:

```sh
npx turbo link
```

## Useful Links

Learn more about the power of Turborepo:

- [Tasks](https://turbo.build/repo/docs/core-concepts/monorepos/running-tasks)
- [Caching](https://turbo.build/repo/docs/core-concepts/caching)
- [Remote Caching](https://turbo.build/repo/docs/core-concepts/remote-caching)
- [Filtering](https://turbo.build/repo/docs/core-concepts/monorepos/filtering)
- [Configuration Options](https://turbo.build/repo/docs/reference/configuration)
- [CLI Usage](https://turbo.build/repo/docs/reference/command-line-reference)

Learn more about shadcn/ui:

- [Documentation](https://ui.shadcn.com/docs)
