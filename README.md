# Flutter Bounty Hunters Business Webpage
Webpage that displays info about the Flutter Bounty Hunters business operations.

## Hugo
This webpage is built with a static site generator called Hugo.

Page content is written as Markdown under `/content`.

Hugo can't do anything without a theme. We've installed a theme called `digitalgarden`. The theme has a large amount of control over where we need to write content, the kind of content that's understood, and the structure of the nav menu.

### Theme
The "digitalgarden" theme is on [GitHub](https://github.com/apvarun/digital-garden-hugo-theme). Check the [example site](https://github.com/apvarun/digital-garden-hugo-theme/tree/main/exampleSite) to see the basics for structuring this directory. Check the [document](https://digital-garden-hugo-theme.vercel.app/articles/installation/) for more detailed information.

The theme forced us to copy `package.json`, `package-lock.json`, and `tailwind.config.js` into the root directory, and then `npm install`. Hugo doesn't inherently require NPM or Tailwind.

The theme wants a global install of `postcss-cli`, e.g., `npm i -g postcss-cli`.

The theme also wants us to deploy the server with `npm run dev` instead of the normal `hugo server` command.

To build for production, either locally or in CI, use `npm i -g postcss-cli && npm run build`.