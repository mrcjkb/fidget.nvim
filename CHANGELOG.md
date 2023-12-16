# Changelog

## [2.0.0](https://github.com/mrcjkb/fidget.nvim/compare/v1.1.0...v2.0.0) (2023-12-16)


### ⚠ BREAKING CHANGES

* reorganize all documentation (fix #144)
* deprecate lsp_name and lsp_id in ProgressMessage
* **progress:** make ignore_empty_message = false the default
* option to position window away from cursor ([#175](https://github.com/mrcjkb/fidget.nvim/issues/175))
* Switch to event-driven LSP progress polling by default
* add stack upwards option ([#160](https://github.com/mrcjkb/fidget.nvim/issues/160))
* rewrite fidget.nvim ([#143](https://github.com/mrcjkb/fidget.nvim/issues/143))
* I told you there would be breaking changes (sorry)

### doc

* reorganize all documentation (fix [#144](https://github.com/mrcjkb/fidget.nvim/issues/144)) ([f7dde2b](https://github.com/mrcjkb/fidget.nvim/commit/f7dde2bd4b9ae95a5fc11c2eed7467331854e219))


### breaking

* rewrite fidget.nvim ([#143](https://github.com/mrcjkb/fidget.nvim/issues/143)) ([50dc5bb](https://github.com/mrcjkb/fidget.nvim/commit/50dc5bb17e375dbc6bcea24db81360fd9d8d5197))


### break

* I told you there would be breaking changes (sorry) ([a09c052](https://github.com/mrcjkb/fidget.nvim/commit/a09c052dc11e92a75ad12aaf109156a858a0d034))


### Features

* add API for dynamically adjusting x_offset ([22b2ed8](https://github.com/mrcjkb/fidget.nvim/commit/22b2ed8f19b9cfc636d162e7478184ff26369926))
* add API function to remove() notification items ([df0caf2](https://github.com/mrcjkb/fidget.nvim/commit/df0caf2e4cf66a984325e4cca3c3e55422d67cd1))
* add default spinner period + improve documentation ([5e89605](https://github.com/mrcjkb/fidget.nvim/commit/5e89605218982fd508a89f2da1f49380fecdc930)), closes [#166](https://github.com/mrcjkb/fidget.nvim/issues/166)
* add Lua API for clearing notifications ([a830e2e](https://github.com/mrcjkb/fidget.nvim/commit/a830e2e1549ca2167c3cb0184d7800fa37035fa8))
* add notification.window.relative option ([37c2b49](https://github.com/mrcjkb/fidget.nvim/commit/37c2b497d9c52d88f17a962d86dc0b7eb447cb6c))
* add poll_once() method to poller ([53f3297](https://github.com/mrcjkb/fidget.nvim/commit/53f32973b7914973b780fe74af38312d58372391))
* add some INFO-level logging to progress and poller ([98047f3](https://github.com/mrcjkb/fidget.nvim/commit/98047f30e454dd36da00eb354506517166cfec7d))
* add stack upwards option ([#160](https://github.com/mrcjkb/fidget.nvim/issues/160)) ([03d2192](https://github.com/mrcjkb/fidget.nvim/commit/03d21920283feba3b79f188f0c7a3f1796bd7a52))
* add type-checking to fidget.notify() ([1dc85e7](https://github.com/mrcjkb/fidget.nvim/commit/1dc85e7a1c12b067658aeec6dec2cc046c231607))
* change Fidget window border color (close [#174](https://github.com/mrcjkb/fidget.nvim/issues/174)) ([b0ca757](https://github.com/mrcjkb/fidget.nvim/commit/b0ca7570c6652766797372734a498b234d9f3648))
* configurable logging path ([430053f](https://github.com/mrcjkb/fidget.nvim/commit/430053fecb6024d87db69bec6d4c95551c2982a6))
* configure LSP progress buffer size (addres [#167](https://github.com/mrcjkb/fidget.nvim/issues/167)) ([5be956d](https://github.com/mrcjkb/fidget.nvim/commit/5be956d940d3ebeb7ea04289382117876c68ce13))
* customize the annotation string for explicit log levels ([dd20c61](https://github.com/mrcjkb/fidget.nvim/commit/dd20c61ba49a9b2b809c8c5742dce83a2a19968d))
* deprecate lsp_name and lsp_id in ProgressMessage ([7be4786](https://github.com/mrcjkb/fidget.nvim/commit/7be478652378b7d52706fd9649997e09a55f9c78))
* ignore message-less messages (fix [#171](https://github.com/mrcjkb/fidget.nvim/issues/171)) ([fe60ce7](https://github.com/mrcjkb/fidget.nvim/commit/fe60ce7a979affda1d9caba08ab44af62ed6d39f))
* integrate with nvim-tree to avoid collisions ([72be8c6](https://github.com/mrcjkb/fidget.nvim/commit/72be8c6b99c8b04c961a71c2a14464bfe5a63faf)), closes [#163](https://github.com/mrcjkb/fidget.nvim/issues/163)
* **internal:** add lsp_client as field to ProgressMessage ([7055343](https://github.com/mrcjkb/fidget.nvim/commit/705534378f791a0e94dba8a5f014ca0709ac7ddb))
* **internal:** return window_id in notification.window.show() ([016aabd](https://github.com/mrcjkb/fidget.nvim/commit/016aabd56e161ca28a512c1f4137878022913963))
* introduce logger.at_level() guard, add timing info to poller ([f10103f](https://github.com/mrcjkb/fidget.nvim/commit/f10103f8f30fed80a7ab07fff5756164fea87c70))
* introduce override_vim_notify option (fix [#157](https://github.com/mrcjkb/fidget.nvim/issues/157)) ([4b666f4](https://github.com/mrcjkb/fidget.nvim/commit/4b666f4d44f55fcbcc1cb27da1b1d4f58bed7078))
* let poller catch and throttle errors to avoid meltdown ([71dd3be](https://github.com/mrcjkb/fidget.nvim/commit/71dd3be2e112237012b6a6133a7d92891bb077fc))
* limit notifications rendering with render_limit ([e8e7952](https://github.com/mrcjkb/fidget.nvim/commit/e8e79523069b21f63f7350280423bdf0669e79ad)), closes [#151](https://github.com/mrcjkb/fidget.nvim/issues/151)
* log to vim.fn.stdpath('cache') instead of 'data' (fix [#94](https://github.com/mrcjkb/fidget.nvim/issues/94)) ([ade2ef1](https://github.com/mrcjkb/fidget.nvim/commit/ade2ef14de92274b43a528fc52b4b5c5a2771c93))
* log warnings about unknown setup options ([45b6bfe](https://github.com/mrcjkb/fidget.nvim/commit/45b6bfed7f94adf8a91330676d05a42082b06b49))
* **notification:** configure skip_history from notification config ([580b4e4](https://github.com/mrcjkb/fidget.nvim/commit/580b4e4ceca2f474be78101b480eb523efe30406))
* notifications level filter ([7161951](https://github.com/mrcjkb/fidget.nvim/commit/7161951a89a526314e7b5a09a3da10873da67fc6))
* **notification:** support notifications history ([93d944f](https://github.com/mrcjkb/fidget.nvim/commit/93d944fd77bd2b6f0a7f6d1a30c8bc0aa5803191))
* option to position window away from cursor ([#175](https://github.com/mrcjkb/fidget.nvim/issues/175)) ([c4a1aff](https://github.com/mrcjkb/fidget.nvim/commit/c4a1aff77af457fd2e9490cd80880f21fb51e25e))
* **progress:** Clear notification group on LspDetach ([883b74f](https://github.com/mrcjkb/fidget.nvim/commit/883b74f03f18b53e27038c5f5de71a5db3e4f676))
* **progress:** omit progress messages from notifications history ([4ca2fb1](https://github.com/mrcjkb/fidget.nvim/commit/4ca2fb1fadea9fbf7203cc4a04d247eb00edd7bd))
* public progress API for non-lsp use cases ([#178](https://github.com/mrcjkb/fidget.nvim/issues/178)) ([d81cc08](https://github.com/mrcjkb/fidget.nvim/commit/d81cc087da109b53b0d067203402a34503e45ccb))
* support ignoring transient tasks (address [#73](https://github.com/mrcjkb/fidget.nvim/issues/73)) ([893ceb3](https://github.com/mrcjkb/fidget.nvim/commit/893ceb3ffdafe5d7baece2b6bc9a8f7ea3b71da5))
* support suppressing notifications while in insert mode ([781c8ab](https://github.com/mrcjkb/fidget.nvim/commit/781c8ab221bcd0d803f7fb3efbe114ad94f00c7f))
* support top-aligned notification window (fidget is vers) ([da354d8](https://github.com/mrcjkb/fidget.nvim/commit/da354d8eba28941bdcb7d57b2b657472d3950609)), closes [#146](https://github.com/mrcjkb/fidget.nvim/issues/146)
* support update_only notifications ([7880df0](https://github.com/mrcjkb/fidget.nvim/commit/7880df0133556697a8efee0278b52c6add32df8a))
* Switch to event-driven LSP progress polling by default ([74b6196](https://github.com/mrcjkb/fidget.nvim/commit/74b619687556a9c339e90894df92fef31ae15958))
* warn user about unknown setup() options (close [#154](https://github.com/mrcjkb/fidget.nvim/issues/154)) ([ff0f59d](https://github.com/mrcjkb/fidget.nvim/commit/ff0f59dce9d8606ed28f43ea8ceb5aa760a3497c))


### Bug Fixes

* 36 ([841ad57](https://github.com/mrcjkb/fidget.nvim/commit/841ad572f860a5ca76923fabbed8a8f5a49dac86))
* Add E565 to window guard whitelist (fix [#93](https://github.com/mrcjkb/fidget.nvim/issues/93)) ([4a444b5](https://github.com/mrcjkb/fidget.nvim/commit/4a444b58ba45bc8c36ec73ede52bf7d660d13ee1))
* also clear notification groups on notification.reset() ([956c8da](https://github.com/mrcjkb/fidget.nvim/commit/956c8da3fa4072e6e00a4d8d4e52b88d887b9cfa))
* **ci:** do not add lemmy-help binary in CI ([e1ecc2d](https://github.com/mrcjkb/fidget.nvim/commit/e1ecc2deb095d29eb2256bebc6c596fd486a8586))
* clean up logging... ([4a4e6e5](https://github.com/mrcjkb/fidget.nvim/commit/4a4e6e570d739a59935ba6c8489183d1b94b36c2))
* correct level used by in-progress and done tasks (fix [#165](https://github.com/mrcjkb/fidget.nvim/issues/165)) ([07371ac](https://github.com/mrcjkb/fidget.nvim/commit/07371ac74c2fbfcc14f99d6dfbb8cb10178fbbea))
* correctly set desc key in nvim_create_autocmd (fix [#145](https://github.com/mrcjkb/fidget.nvim/issues/145)) ([d3edb8d](https://github.com/mrcjkb/fidget.nvim/commit/d3edb8d2f9958cdbe6d1a51bfff9d8761aa46f20))
* **doc:** generate link instead of tag in ToC ([3f5a5bb](https://github.com/mrcjkb/fidget.nvim/commit/3f5a5bbf57cf286f4369a273a0a44f442be79c32))
* docs badge link ([fd95ef3](https://github.com/mrcjkb/fidget.nvim/commit/fd95ef3799e6b9b412a6966b14a0902457d6d0d2))
* don't render any name line if name and icon are empty ([8ec626c](https://github.com/mrcjkb/fidget.nvim/commit/8ec626cd17f8de073ebd3134fb674e8c0d760a83))
* inherit from default when adding notification configs (fix [#169](https://github.com/mrcjkb/fidget.nvim/issues/169)) ([bd0b8b6](https://github.com/mrcjkb/fidget.nvim/commit/bd0b8b644d4fb293dc4df2718b1f2df3abd90767))
* optins -&gt; options ([#147](https://github.com/mrcjkb/fidget.nvim/issues/147)) ([a03c0d0](https://github.com/mrcjkb/fidget.nvim/commit/a03c0d03d8c157efe5a75b2326b47bdc7406cbbf))
* **progress:** make ignore_empty_message = false the default ([5aa7cd3](https://github.com/mrcjkb/fidget.nvim/commit/5aa7cd32c2446fe4a058d6f991c6579c3fdb4c76))
* Read correct option name ([2dfaf28](https://github.com/mrcjkb/fidget.nvim/commit/2dfaf28c4738e91fe2363ad2d19b36c87ab3b4c6))
* right-justify by padding with spaces in Lua, rather than using :right ([#158](https://github.com/mrcjkb/fidget.nvim/issues/158)) ([788f3bc](https://github.com/mrcjkb/fidget.nvim/commit/788f3bcc4ecb07f19d86fa35d7cb0e10dafbf2c3))
* scrolloff breaks notification window ([#155](https://github.com/mrcjkb/fidget.nvim/issues/155)) ([b8ec74a](https://github.com/mrcjkb/fidget.nvim/commit/b8ec74a031febd52f64559b15002d5dee08e4791))
* the emoji in the README lol ([5be46c8](https://github.com/mrcjkb/fidget.nvim/commit/5be46c8aeb5d37e1da20cd613b286329ca2a4fca))
* use byte-index instead of strdisplaywidth when computing highlights ([4bb8d83](https://github.com/mrcjkb/fidget.nvim/commit/4bb8d83504a0699f000dbe3074c5cf74596b6072)), closes [#153](https://github.com/mrcjkb/fidget.nvim/issues/153)
* vimdocs ([197014c](https://github.com/mrcjkb/fidget.nvim/commit/197014c6e1e2f4a4c9e61b466b6eba7ab4893051))

## [1.1.0](https://github.com/j-hui/fidget.nvim/compare/v1.0.0...v1.1.0) (2023-12-08)


### Features

* public progress API for non-lsp use cases ([#178](https://github.com/j-hui/fidget.nvim/issues/178)) ([d81cc08](https://github.com/j-hui/fidget.nvim/commit/d81cc087da109b53b0d067203402a34503e45ccb))


### Bug Fixes

* **ci:** do not add lemmy-help binary in CI ([e1ecc2d](https://github.com/j-hui/fidget.nvim/commit/e1ecc2deb095d29eb2256bebc6c596fd486a8586))
* **doc:** generate link instead of tag in ToC ([3f5a5bb](https://github.com/j-hui/fidget.nvim/commit/3f5a5bbf57cf286f4369a273a0a44f442be79c32))
* docs badge link ([fd95ef3](https://github.com/j-hui/fidget.nvim/commit/fd95ef3799e6b9b412a6966b14a0902457d6d0d2))

## [1.0.0](https://github.com/j-hui/fidget.nvim/compare/v0.0.0...v1.0.0) (2023-12-07)


### ⚠ BREAKING CHANGES

* reorganize all documentation (fix #144)

### doc

* reorganize all documentation (fix [#144](https://github.com/j-hui/fidget.nvim/issues/144)) ([f7dde2b](https://github.com/j-hui/fidget.nvim/commit/f7dde2bd4b9ae95a5fc11c2eed7467331854e219))


### Bug Fixes

* the emoji in the README lol ([5be46c8](https://github.com/j-hui/fidget.nvim/commit/5be46c8aeb5d37e1da20cd613b286329ca2a4fca))
