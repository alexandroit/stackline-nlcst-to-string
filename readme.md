# @stackline/nlcst-to-string

> nlcst utility to transform a tree to a string.

[![npm version](https://img.shields.io/npm/v/@stackline/nlcst-to-string.svg?style=flat-square)](https://www.npmjs.com/package/@stackline/nlcst-to-string)
[![license](https://img.shields.io/npm/l/@stackline/nlcst-to-string.svg?style=flat-square)](https://github.com/alexandroit/stackline-nlcst-to-string)
[![GitHub repository](https://img.shields.io/badge/GitHub-repository-181717?style=flat-square&logo=github)](https://github.com/alexandroit/stackline-nlcst-to-string)
[![Docs](https://img.shields.io/badge/docs-alexandro.net-0f766e?style=flat-square)](https://alexandro.net/docs/vanilla/nlcst-to-string/)
[![Reddit community](https://img.shields.io/badge/community-r%2FStackline-ff4500?style=flat-square&logo=reddit&logoColor=white)](https://www.reddit.com/r/Stackline/)

**[Documentation](https://alexandro.net/docs/vanilla/nlcst-to-string/)** | **[npm](https://www.npmjs.com/package/@stackline/nlcst-to-string)** | **[Issues](https://github.com/alexandroit/stackline-nlcst-to-string/issues)** | **[Repository](https://github.com/alexandroit/stackline-nlcst-to-string)**

**Current package version:** `1.0.2`

---

## Why this package?

`@stackline/nlcst-to-string` is the Stackline-maintained distribution of `nlcst-to-string@3.1.1`. It is an independent continuation of [nlcst-to-string](https://github.com/syntax-tree/nlcst-to-string); original authors and licenses remain credited below.

## Compatibility

| Item | Value |
| :--- | :--- |
| Package | `@stackline/nlcst-to-string@1.0.2` |
| API target | `nlcst-to-string@3.1.1` |
| Supported Node.js | `See supported framework requirements` |
| License | `MIT` |
| Module type | `module` |
| Main entry | `index.js` |
| Types | `index.d.ts` |
| Runtime dependencies | `@types/nlcst` |

## Installation

```bash
npm install @stackline/nlcst-to-string
```

Preserve existing imports and plugin resolution with an npm alias:

```bash
npm install nlcst-to-string@npm:@stackline/nlcst-to-string
```

## Usage and API reference

### nlcst-to-string


[nlcst][] utility to serialize a node.

## Contents

*   [What is this?](#what-is-this)
*   [When should I use this?](#when-should-i-use-this)
*   [Install](#install)
*   [Use](#use)
*   [API](#api)
    *   [`toString(value[, separator])`](#tostringvalue-separator)
*   [Types](#types)
*   [Compatibility](#compatibility)
*   [Contribute](#contribute)
*   [License](#license)

## What is this?

This package is a utility that takes [nlcst][] nodes and gets their plain-text
value.

## When should I use this?

This is a small utility that is useful when you’re dealing with ASTs.

## Install

This package is [ESM only][esm].
In Node.js (version 14.14+ and 16.0+), install with [npm][]:

```sh
npm install @stackline/nlcst-to-string
```

In Deno with [`esm.sh`][esmsh]:

```js
import {toString} from 'https://esm.sh/nlcst-to-string@3'
```

In browsers with [`esm.sh`][esmsh]:

```html
<script type="module">
  import {toString} from 'https://esm.sh/nlcst-to-string@3?bundle'
</script>
```

## Use

```js
import {toString} from '@stackline/nlcst-to-string'

console.log(
  toString({
    type: 'WordNode',
    children: [
      {type: 'TextNode', value: 'AT'},
      {type: 'PunctuationNode', value: '&'},
      {type: 'TextNode', value: 'T'}
    ]
  })
) // => 'AT&T'
```

## API

This package exports the identifier [`toString`][tostring].
There is no default export.

### `toString(value[, separator])`

Get the text content of a node or list of nodes.

Prefers the node’s plain-text fields, otherwise serializes its children, and
if the given value is an array, serialize the nodes in it.

###### Parameters

*   `node` ([`Node`][node] or `Array<Node>`)
    — node to serialize.
*   `separator` (`string`, default: `''`)
    — value to delimit each item

###### Returns

Result (`string`).

## Types

This package is fully typed with [TypeScript][].
It exports no additional types.

## Compatibility

Projects maintained by the unified collective are compatible with all maintained
versions of Node.js.
As of now, that is Node.js 14.14+ and 16.0+.
Our projects sometimes work with older versions, but this is not guaranteed.

## Contribute

See [`contributing.md`][contributing] in [`syntax-tree/.github`][health] for
ways to get started.
See [`support.md`][support] for ways to get help.

This project has a [code of conduct][coc].
By interacting with this repository, organization, or community you agree to
abide by its terms.

## License

[MIT][license] © [Titus Wormer][author]



[build-badge]: https://github.com/syntax-tree/nlcst-to-string/workflows/main/badge.svg

[build]: https://github.com/syntax-tree/nlcst-to-string/actions

[coverage-badge]: https://img.shields.io/codecov/c/github/syntax-tree/nlcst-to-string.svg

[coverage]: https://codecov.io/github/syntax-tree/nlcst-to-string

[downloads-badge]: https://img.shields.io/npm/dm/nlcst-to-string.svg

[downloads]: https://www.npmjs.com/package/nlcst-to-string

[size-badge]: https://img.shields.io/bundlephobia/minzip/nlcst-to-string.svg

[size]: https://bundlephobia.com/result?p=nlcst-to-string

[sponsors-badge]: https://opencollective.com/unified/sponsors/badge.svg

[backers-badge]: https://opencollective.com/unified/backers/badge.svg

[collective]: https://opencollective.com/unified

[chat-badge]: https://img.shields.io/badge/chat-discussions-success.svg

[chat]: https://github.com/syntax-tree/unist/discussions

[npm]: https://docs.npmjs.com/cli/install

[esm]: https://gist.github.com/sindresorhus/a39789f98801d908bbc7ff3ecc99d99c

[esmsh]: https://esm.sh

[typescript]: https://www.typescriptlang.org

[license]: license

[author]: https://wooorm.com

[health]: https://github.com/syntax-tree/.github

[contributing]: https://github.com/syntax-tree/.github/blob/main/contributing.md

[support]: https://github.com/syntax-tree/.github/blob/main/support.md

[coc]: https://github.com/syntax-tree/.github/blob/main/code-of-conduct.md

[nlcst]: https://github.com/syntax-tree/nlcst

[node]: https://github.com/syntax-tree/nlcst#nodes

[tostring]: #tostringvalue-separator

## Credits and original authors

- Original project: [nlcst-to-string](https://github.com/syntax-tree/nlcst-to-string).
- Titus Wormer.
- Kenichiro Murata.
- Copyright (c) 2014 Titus Wormer <tituswormer@gmail.com>.
- Stackline maintenance: [Alexandro Paixao Marques](https://www.linkedin.com/in/aleinfo/) and [Stackline contributors](https://github.com/alexandroit).

Original copyright, license notices and contributor acknowledgements remain part of this distribution. Stackline maintenance does not replace authorship of the original work.

## Community and Links

- [Stackline website](https://alexandro.net/)
- [GitHub projects](https://github.com/alexandroit)
- [npm packages](https://www.npmjs.com/~alex360qc)
- [Reddit community — r/Stackline](https://www.reddit.com/r/Stackline/)
- [Maintainer LinkedIn](https://www.linkedin.com/in/aleinfo/)

Use this repository's issue tracker for reproducible bugs and feature requests. Join r/Stackline for examples, usage questions and release discussions.
