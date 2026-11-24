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

#### WordPress core

Recent patches to [wordpress-develop](https://github.com/WordPress/wordpress-develop), each linked to its Trac ticket:

- REST API: assign the default category when a post's categories are emptied ([PR #16101](https://github.com/WordPress/wordpress-develop/pull/16101), [Trac #66742](https://core.trac.wordpress.org/ticket/66742))
- Bulk Edit: allow removing Uncategorized and reset category states ([PR #16090](https://github.com/WordPress/wordpress-develop/pull/16090), [Trac #59374](https://core.trac.wordpress.org/ticket/59374))
- Quick Edit: allow removing all categories from a post ([PR #16088](https://github.com/WordPress/wordpress-develop/pull/16088), [Trac #66729](https://core.trac.wordpress.org/ticket/66729))
- Taxonomy: add `search_columns` support to `WP_Term_Query` and search term descriptions in the admin ([PR #14138](https://github.com/WordPress/wordpress-develop/pull/14138), [Trac #66281](https://core.trac.wordpress.org/ticket/66281))
- Editor: remove the unused `wp_get_state_style_with_fallback_dimension_styles()` ([PR #14121](https://github.com/WordPress/wordpress-develop/pull/14121), [Trac #66274](https://core.trac.wordpress.org/ticket/66274))
- Comments: update the "Mine" view count after AJAX moderation actions ([PR #14114](https://github.com/WordPress/wordpress-develop/pull/14114), [Trac #66272](https://core.trac.wordpress.org/ticket/66272))
- Comments: hide zero-count status filters on the Comments list table ([PR #14056](https://github.com/WordPress/wordpress-develop/pull/14056), [Trac #66260](https://core.trac.wordpress.org/ticket/66260))
- REST API: fix a fatal error in `rest_filter_response_fields()` with object response data ([PR #13931](https://github.com/WordPress/wordpress-develop/pull/13931), [Trac #66230](https://core.trac.wordpress.org/ticket/66230))
- Embeds: strip an existing `#?secret=` fragment before appending a new one in `wp_filter_oembed_result()` ([PR #13868](https://github.com/WordPress/wordpress-develop/pull/13868), [Trac #66218](https://core.trac.wordpress.org/ticket/66218))
- I18N: validate MO header and table offsets before use in `WP_Translation_File_MO` ([PR #13850](https://github.com/WordPress/wordpress-develop/pull/13850), [Trac #66217](https://core.trac.wordpress.org/ticket/66217))
- Multisite: fix invalid markup and clarify docs for the `myblogs_options` filter ([PR #13849](https://github.com/WordPress/wordpress-develop/pull/13849), [Trac #66216](https://core.trac.wordpress.org/ticket/66216))

#### Tools I use

PHP · JavaScript/React · `@wordpress/scripts` · block.json / Block API v3 · block supports & deprecations · Interactivity API · Font Library · REST API · WP-CLI · PHPUnit
