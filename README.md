# catchen.me [![Netlify Status](https://api.netlify.com/api/v1/badges/d31fdc8f-877d-4986-911e-41cd7804bb09/deploy-status)](https://app.netlify.com/sites/catchen/deploys)

This is the source code that can be compiled into the static site behind [catchen.me](https://catchen.me).

## Compile

To compile the source code into static site pages, we need to use [Harp](https://github.com/sintaxi/harp).

Install Harp and other dependencies with `yarn install`. Compile with `yarn build`. Develop with `yarn start` on localhost.

## Deploy

The site deploys automatically to Netlify on every push to `main`.

## Localization

Pages are served under `/en/` and `/zh/` URL prefixes. The base data lives in `public/_data.json` (English). Chinese overrides are in `public/zh/_data.json` and are deep-merged on top of the base at render time.

## CSS

Bootstrap is compiled from SCSS source so unused modules can be excluded. To enable additional Bootstrap components, add the corresponding `@import` to `public/css/bootstrap-custom.scss`.
