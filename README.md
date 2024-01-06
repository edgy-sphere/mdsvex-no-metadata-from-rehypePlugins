# MDsveX no metadata from `rehypePlugins`

## Issue

Adding metadata via a plugin in `rehypePlugins`, unlike in `remarkPlugins`, does not work.

## Reproduction

Repo link: https://github.com/edgy-sphere/mdsvex-no-metadata-from-rehypePlugins

- Clone: `git clone https://github.com/edgy-sphere/mdsvex-no-metadata-from-rehypePlugins.git`
- Install dependencies: `npm i`
- Start the dev server: `npm run dev`
- Visit `localhost:5173` in your browser.

In this repo, at `svelte.config.js` the metadata-modifying plugins (using `vFile.data.fm`) are given to the mdsvex preprocessor, but `+page.svelte`, which uses the dummy `post.svx`, only receives the additional metadata set at `remarkPlugins`.

## Workaround / Solution

I could not come to understand how this, or any svelte plugin in general, works, therefore I sadly cannot present any material help; nor do I know whether this might be intentional or if I might have written improper code.
