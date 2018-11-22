[![Build Status](https://badgen.net/travis/danoc/clickable-box)](https://travis-ci.com/danoc/clickable-box) [![Code Coverage](https://badgen.net/codecov/c/github/danoc/clickable-box)](https://codecov.io/gh/danoc/clickable-box)

# `ClickableBox`

**Problem:** It's [very hard](https://www.scottohara.me/blog/2018/10/03/unbutton-buttons.html) to remove all styles from HTML `button` elements.

It's also hard to create clickable `div`s that are accessible.

**Solution:** The `ClickableBox` component allows you to add `onClick` to HTML elements without sacrificing accessibility.

## Install

You can install `ClickableBox` with NPM or Yarn.

```bash
npm install clickable-box --save-exact
```

```bash
yarn add clickable-box --exact
```

We encourage pinning the version number until `ClickableBox` reaches `1.0.0`. We may ship breaking changes in `0.x.x` versions.

## Props

There are a few props that are built into `ClickableBox`:

| prop      | type                                            | description                                       |
| --------- | ----------------------------------------------- | ------------------------------------------------- |
| `onClick` | `function` \| _required_                        | The action to perform when the element is pressed |
| `is`      | `string`, `React.Element` \| defaults to: `div` | The element to render                             |
| `ref`     | `React.Ref`                                     | Provides access to the React element              |

You can pass any custom prop as well since this component spreads all of the props on the rendered element.
