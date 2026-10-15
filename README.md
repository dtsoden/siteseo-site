# siteseoai-site

The public page for [siteseoai](https://github.com/dtsoden/siteseoai), served at
https://siteseoai.davidsoden.com from Cloudflare, as a Worker that serves static
files. `wrangler.jsonc` holds the project name and the custom domain.

Everything served lives in `site/`. It is plain HTML with no build step.

The release line under the main heading reads the latest release from the
GitHub API in the visitor's browser, so publishing a siteseoai release updates the
page without a redeploy.

Deploy after changing anything in `site/`:

```
npx wrangler deploy
```

The brand files are in `site/` (`icon.svg`, `favicon.ico`, the PNG icons) and
`site/brand/` (`logo.svg` for light backgrounds, `logo-dark.svg` for dark). The
wordmark is set in Inter Bold, converted to outlines.
