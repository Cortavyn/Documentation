# Cortavyn Documentation

Public documentation for [Cortavyn](https://github.com/Cortavyn/Cortavyn), built with [Nimbus](https://nimbus-docs.com/).

## Local development

Requires Node.js 22.12 or later and pnpm.

```shell
pnpm install
pnpm dev
```

Validate content and produce a static release build with:

```shell
pnpm lint:docs
pnpm typecheck
pnpm build
```

## Deployment

Cloudflare Workers Builds should use `pnpm install --frozen-lockfile` and `pnpm deploy`. Configure `main` as the production branch; Cloudflare creates previews for other branches.

The Worker name is `cortavyn-documentation`. In the Cloudflare dashboard, attach the custom domain `docs.cortavyn.org` to that Worker after the first production deployment.

## License

Documentation is licensed under [Apache-2.0](LICENSE).

