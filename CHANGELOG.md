# Change Log

## [1.1.0] 2021-03-19
### Bug fixing
- Rename `master` branch to `main`
- To make a lot of our changes, we've followed the instructions from here (minus the `colors` and `font-sizes`): https://tailwindcss.com/docs/upgrading-to-v2
  - For the colors, the only change that we made, is the fact that we've added all Tailwind CSS colors to our `tailwind.config.js` files, and inside our product, all `{type}-gray-{number}` classes were renamed to `{type}-blueGray-{number}`
  - After that, we've changed `{type}-blueGray-{number}` to `{type}-blueGray-{lower-number}`, i.e. (`100` became `50`, `200` became `100`, ..., `900` became `800`)
    - You can achieve this, by search in your whole project for `blueGray-100` and replace it with `blueGray-50`
    - Then, you search in your whole project for `blueGray-200` and replace it with `blueGray-100`
    - Then, you search in your whole project for `blueGray-300` and replace it with `blueGray-200`
    - Then, you search in your whole project for `blueGray-400` and replace it with `blueGray-300`
    - Then, you search in your whole project for `blueGray-500` and replace it with `blueGray-400`
    - Then, you search in your whole project for `blueGray-600` and replace it with `blueGray-500`
    - Then, you search in your whole project for `blueGray-700` and replace it with `blueGray-600`
    - Then, you search in your whole project for `blueGray-800` and replace it with `blueGray-700`
    - Then, you search in your whole project for `blueGray-900` and replace it with `blueGray-800`
  - For the colors, the only change that we made, is the fact that we've added all Tailwind CSS colors to our `tailwind.config.js` files, and inside our product, all `{type}-blue-{number}` classes were renamed to `{type}-lightBlue-{number}`
  - For the colors, the only change that we made, is the fact that we've added all Tailwind CSS colors to our `tailwind.config.js` files, and inside our product, all `{type}-green-{number}` classes were renamed to `{type}-emerald-{number}`
- `lg:bg-transparent` is not working anymore, so we've changed it with `lg:bg-opacity-0`
- https://github.com/creativetimofficial/notus-angular/issues/4
- https://github.com/creativetimofficial/notus-js/issues/4
- https://github.com/creativetimofficial/notus-js/pull/5
- https://github.com/creativetimofficial/notus-js/pull/6
- https://github.com/creativetimofficial/notus-nextjs/issues/6
- https://github.com/creativetimofficial/notus-nextjs/issues/7
- https://github.com/creativetimofficial/notus-nextjs/issues/8
- https://github.com/creativetimofficial/notus-react/issues/3
- https://github.com/creativetimofficial/notus-svelte/issues/3
- https://github.com/creativetimofficial/notus-svelte/issues/6
- https://github.com/creativetimofficial/vue-notus/pull/4/
### Major style changes
- The upgrade of Tailwind CSS from version 1 to version 2, will cause multiple style changes, check them out on the official Tailwind CSS websites:
  - https://blog.tailwindcss.com/tailwindcss-v2
  - https://tailwindcss.com/
  - https://tailwindcss.com/docs/upgrading-to-v2
### Deleted components
### Added components
### Deleted dependencies
- `@tailwindcss/custom-forms`
### Added dependencies
- `@tailwindcss/forms` (replaces `@tailwindcss/custom-forms`)
- `postcss`
- `autoprefixer`
### Updated dependencies
```
@fortawesome/fontawesome-free    5.14.0   →    5.15.3
browser-sync                    2.26.12   →   2.26.14
tailwindcss                      1.8.10   →     2.0.4
```
### Warning
_On a clean install there may be some warnings from request, chokidar, fsevents - they come from node_modules, and they do not affect the product at all._

## [1.0.0] 2020-09-29
### Original Release
- Started project from [Tailwind Starter Kit by Creative Tim](https://www.creative-tim.com/learning-lab/tailwind-starter-kit/presentation?ref=njs-changelog)
- Added design from Tailwind Starter Kit by Creative Tim
