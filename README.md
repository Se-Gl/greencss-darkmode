# A classy way to write sustainable CSS

This is a darkmode add-on for the [greenCSS library](https://www.npmjs.com/package/greencss).

[![Prettier Code Style](https://github.com/Se-Gl/greencss-darkmode/actions/workflows/prettier.yml/badge.svg)](https://github.com/Se-Gl/greencss-darkmode/actions/workflows/prettier.yml)
[![Downloads p/week](https://badgen.net/npm/dw/@greencss/darkmode)](https://badgen.net/npm/dw/@greencss/darkmode)
[![NPM version](https://badgen.net/npm/v/@greencss/darkmode)](https://badgen.net/npm/v/@greencss/darkmode)
[![License](https://badgen.net/npm/license/@greencss/darkmode)](https://badgen.net/npm/license/@greencss/darkmode)

![greencss logo](./information/greencss-logo_dark.svg)

## Getting started

```
npm i @greencss/darkmode
```

## Initialisation

- Import all greenCSS and darkmode classes into your project.

```
import 'greencss/css/greencss.css'.
import '@greencss/darkmode/css/greencss.css'
```

- If you only want to use the dark mode colors, for example, import only the category into your project that you need.

```
...
import '@greencss/darkmode/css/classes/color/color.css'
```

Currently, the following categories are available:

- background/background.css
- borders/borders.css
- color/color.css
- effects/effects.css
- filters/filters.css
- flex-grow/flex-grow.css
- interactivity/interactivity.css
- layout/layout.css
- sizing/sizing.css
- spacing/spacing.css
- svg/svg.css
- tables/tables.css
- transforms/transforms.css
- typography/typography.css

You will find more information about the [CSS categories](https://www.greencss.dev/docs) here.

## Lightweight Version

Instead of the normal version, you can also import a lightweight minified version.

```
import '@greencss/darkmode/css/minified/greencss.css'
```

Compact imports also work with categories:

```
import '@greencss/darkmode/css/minified/classes/color/color.css'
```

## Before you code

1. Install the greenCSS library and import it into your project. _If you have not done yet_
2. Install the greenCSS darkmode add-on and import it into your project. _If you have not done yet_
3. Create your personal reset file to adjuste HTML elements according to your needs. _If you have not done yet_
4. Dark mode does not work out of the box. You must specify the dark mode settings in your project. Here we can not make a guide, because this is unique to each project or framework.

```
import 'greencss/css/greencss.css'.
import '@greencss/darkmode/css/greencss.css'
import 'path-to-your-reset.css-file'.
```

## How it works

All greenCSS classes have the same structure. An explanation of this principle can be given with the help of the examples below.

```html
<p class="text-blue dark:text-blue-10">a blue text and a blue-10 text for the dark mode state</p>
```

If the text colour for an element is to be changed on small screens only (0px - 480px), the class is inserted with a prefix called "sm:".

```html
<p class="text-blue dark:text-blue-10 sm:text-purple dark:sm:text-purple-10">
  a purple text for small screens with a dark mode color
</p>
```

In addition to the responsive classes, all dark mode classes also have active, focus and hover classes, which can be combined as desired. Just add the `dark:` prefix in front of every individual class.

```html
<p class="text-blue hover:text-orange dark:text-blue-10 dark:hover:text-orange-10">
  Different text colours and different states for all screens
</p>
```

## Contribute

You want to collaborate? Have a look at the documentation in the information folder.

For commits, use semantig writing:

| Commit                                                             |      Usage       |
| ------------------------------------------------------------------ | :--------------: |
| fix(pencil): stop graphite breaking when too much pressure applied |   Fix Release    |
| feat(pencil): add 'graphiteWidth' option                           | Feature Release  |
| perf(pencil): remove graphiteWidth option                          | Breaking Release |

## Useful links

- [greenCSS library](https://www.npmjs.com/package/greencss)
- [Basic usage](https://www.greencss.dev/docs/activate-basic-usage)
- [Example: Responsive Hero Section](https://www.greencss.dev/blog/how-to-create-a-responsive-hero-section)
- [greenCSS animations](https://www.greencss.dev/examples/animation)
- [greenCSS color schema](https://www.greencss.dev/brand/colours)
- [greenCSS blog](https://www.greencss.dev/blog)
- [greenCSS categories](https://www.greencss.dev/docs)
