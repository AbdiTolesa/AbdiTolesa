### Hi, I'm Abdi 👋

WordPress engineer focused on plugin development and the **block editor (Gutenberg)**. I build blocks, editor sidebars and settings UIs in React on top of `@wordpress/*` packages, and the PHP and REST APIs behind them.

#### Gutenberg

- **[quote-blocks](https://github.com/AbdiTolesa/quote-blocks)**: a custom block with five layout variations and a variation picker. It uses core typography supports with the **Font Library** (it replaced a Google Fonts API integration, with a block deprecation that migrates existing content), puts its style controls in core's Styles tab panels (`InspectorControls` groups), and has an **Interactivity API** copy-to-clipboard button (`viewScriptModule`, generator actions, context).
- **[Rank Math SEO](https://wordpress.org/plugins/seo-by-rank-math/)**: I work on the blocks that ship with the plugin, used on millions of sites:
  - **FAQ block**: made the answer field keyboard-accessible, and fixed its editor layout on mobile.
  - **Table of Contents block**: added an extensibility filter so third-party heading blocks are included.
  - **TOC, FAQ, HowTo and Schema blocks**: fixed block translations not loading.
  - **Local Business and Related Posts blocks** (Pro): fixed both getting stuck on a loading spinner.
  - **Migration**: convert All in One SEO FAQ blocks to Rank Math FAQ blocks on import.
  - **Editor compatibility**: fixed a fatal error when the schema blocks loaded in the Site Editor and Customizer, and fixed the "Fix with AI" tool breaking Gallery blocks.
- **[Formidable Forms](https://wordpress.org/plugins/formidable/)**: contributions to its Form block:
  - [#2194](https://github.com/Strategy11/formidable-forms/pull/2194): the server-rendered block now applies the editor's **Additional CSS class(es)** setting.
  - [#1111](https://github.com/Strategy11/formidable-forms/pull/1111): moved the block off the deprecated `wp.components.ServerSideRender` to `wp.serverSideRender`.

#### Tools I use

PHP · JavaScript/React · `@wordpress/scripts` · block.json / Block API v3 · block supports & deprecations · Interactivity API · Font Library · REST API · WP-CLI · PHPUnit
