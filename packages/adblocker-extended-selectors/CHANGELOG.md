# v1.23.0 (Mon Oct 18 2021)

#### :nut_and_bolt: Dependencies

- Bump jsdom from 17.0.0 to 18.0.0 [#2267](https://github.com/cliqz-oss/adblocker/pull/2267) ([@dependabot[bot]](https://github.com/dependabot[bot]))

#### Authors: 1

- [@dependabot[bot]](https://github.com/dependabot[bot])

---

# v1.22.7 (Wed Sep 22 2021)

#### :house: Internal

- Bump typescript [#2243](https://github.com/cliqz-oss/adblocker/pull/2243) ([@remusao](https://github.com/remusao))

#### :nut_and_bolt: Dependencies

- Bump @types/node from 15.6.1 to 16.9.6 [#2235](https://github.com/cliqz-oss/adblocker/pull/2235) ([@dependabot[bot]](https://github.com/dependabot[bot]))

#### Authors: 2

- [@dependabot[bot]](https://github.com/dependabot[bot])
- Rémi ([@remusao](https://github.com/remusao))

---

# v1.22.5 (Wed Aug 25 2021)

#### :nut_and_bolt: Dependencies

- Bump jsdom from 16.7.0 to 17.0.0 [#2175](https://github.com/cliqz-oss/adblocker/pull/2175) ([@dependabot[bot]](https://github.com/dependabot[bot]))

#### Authors: 1

- [@dependabot[bot]](https://github.com/dependabot[bot])

---

# v1.22.3 (Thu Jul 29 2021)

#### :nut_and_bolt: Dependencies

- Bump @types/mocha from 8.2.3 to 9.0.0 [#2062](https://github.com/cliqz-oss/adblocker/pull/2062) ([@dependabot[bot]](https://github.com/dependabot[bot]))

#### Authors: 1

- [@dependabot[bot]](https://github.com/dependabot[bot])

---

# v1.22.2 (Sun Jun 20 2021)

#### :nut_and_bolt: Dependencies

- Bump mocha from 8.4.0 to 9.0.0 [#1989](https://github.com/cliqz-oss/adblocker/pull/1989) ([@dependabot[bot]](https://github.com/dependabot[bot]))

#### Authors: 1

- [@dependabot[bot]](https://github.com/dependabot[bot])

---

# v1.21.0 (Sun May 30 2021)

#### :rocket: New Feature

- Bump Electron to v13.x and Puppeteer to v9.x [#1967](https://github.com/cliqz-oss/adblocker/pull/1967) ([@remusao](https://github.com/remusao))

#### :house: Internal

- Bump lock file to fix some security issue [#1922](https://github.com/cliqz-oss/adblocker/pull/1922) ([@remusao](https://github.com/remusao))

#### Authors: 1

- Rémi ([@remusao](https://github.com/remusao))

---

# v1.20.5 (Tue May 04 2021)

#### :bug: Bug Fix

- build(deps-dev): bump @types/node from 14.14.41 to 15.0.0 ([@dependabot-preview[bot]](https://github.com/dependabot-preview[bot]))

#### :nut_and_bolt: Dependencies

- build(deps-dev): bump auto from 10.25.1 to 10.25.2 [#1892](https://github.com/cliqz-oss/adblocker/pull/1892) ([@dependabot-preview[bot]](https://github.com/dependabot-preview[bot]))
- build(deps): bump tldts-experimental from 5.7.29 to 5.7.30 [#1889](https://github.com/cliqz-oss/adblocker/pull/1889) ([@dependabot-preview[bot]](https://github.com/dependabot-preview[bot]))
- build(deps-dev): bump @types/node from 14.14.41 to 15.0.0 [#1888](https://github.com/cliqz-oss/adblocker/pull/1888) ([@dependabot-preview[bot]](https://github.com/dependabot-preview[bot]))

#### Authors: 1

- [@dependabot-preview[bot]](https://github.com/dependabot-preview[bot])

---

# v1.20.0 (Thu Jan 21 2021)

### Release Notes

#### Initial support for extended CSS selectors (a.k.a. procedural filters) ([#1574](https://github.com/cliqz-oss/adblocker/pull/1574))

Add initial support for extended CSS selectors (a.k.a. procedural filters) as well as the `:remove()` modifier for element hiding rules (note: the already supported `:style` modified now also works with extended CSS selectors). The following new pseudo-classes are implemented: `:has` (and its alias `:if`), `:has-text` (both string and RegExp literals), and `:not` (whenever its argument is also an extended selector, otherwise fallback to native implementation).

Caveats:
* Loading of extended css filters is disabled by default and needs to be toggled using the `loadExtendedSelectors` option while [initializing the blocker instance](https://github.com/cliqz-oss/adblocker/blob/3361723138f40c3cb96b4c6e611f2b030f75d891/packages/adblocker-webextension-example/background.ts#L61).
* These news selectors are currently only supported by `WebExtensionBlocker` (support for Puppeteer, Electron and Playwright is not planned at this time but help from the community would be greatly appreciated).

Miscellaneous changes:
* Removal of unused `injectCSSRule` helper.
* Replace Closure compiler by Terser.

---

#### :rocket: New Feature

- Initial support for extended CSS selectors (a.k.a. procedural filters) [#1574](https://github.com/cliqz-oss/adblocker/pull/1574) ([@remusao](https://github.com/remusao))

#### Authors: 1

- Rémi ([@remusao](https://github.com/remusao))
