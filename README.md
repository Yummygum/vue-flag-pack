# Flagpack

Flagpack contains 260+ flag icons to easily use within your code project. Flagpack is an open source project and available for JavaScript frameworks/libraries Angular, Vue and React.

![Flagpack. 260+ easily implementable flag icons to use in your design or code project. Open Source. Available for Sketch, Figma, Angular, Vue, and React. [www.flagpack.xyz](http://www.flagpack.xyz). Made with love by Yummygum. Graphic showing a list with the flags of Argentina, Croatia, Estonia, Kenia, Netherlands, and Scotland.](https://flagpack.xyz/meta-image.png)

[View documentation on flagpack.xyz](https://flagpack.xyz/docs/)

## vue-flagpack
Flagpack for Vue is created using Vue v2.5.11. The Flagpack component has not been tested for compatibility with older version of Vue.

## Installation

```bash
npm install vue-flagpack
```

## Usage
### As a plugin
```js
import Vue from 'vue'
import Flag from 'vue-flagpack'

Vue.use(Flag, {
  name: 'Flag'
})
```

In your template:
```html
<template>
  <vue-flagpack code="NL" />
</template>
```

### Import straight away
```js
import { Flag } from 'vue-flagpack'

Vue.component('flag-nl', {
  components: {
    Flag
  },
  template: `
    <Flag code="NL" />
  `
})
```

### Via UNPKG network
```html
<script src="https://unpkg.com/vue-flagpack@latest/dist/vue-flag-rollup.cjs.js"></script>
<script>
const instance = new Vue({
  el: '#app',
  components: {
    'Flag': Flag.Flag
  },
})

// or
instance.use(Flag)
</script>
```

## Available plugin options

| Key   | Value   | Required | Default |
|-------|-------|------|------|
| name |  String | false | vue-flagpack |



## Available component configurations — Props

| Key   | Value   | Required | Default | Format |
|-------|-------|------|------|------|
| code |  String | false | 'NL' | [See all codes](https://flagpack.xyz/docs/flag-index/) |
| size |  String | false | 'L' | 'S', 'M' or 'L' |
| className |  String | false | - | - |
| hasDropShadow |  Boolean | false | false | - |
| hasBorder |  Boolean | false | true | - |
| hasBorderRadius | Boolean | false | true | - |
| gradient |  String | false | '' | 'top-down', 'real-linear' or 'real-circular' |



## Build Dist

```bash
# install dependencies
npm install

# build for prod
npm run build

# build with watcher for dev
npm run dev
```

## Releasing
To release a new version you'll need to make sure all changes commits are done and pushed. After that you'll need to decide which release type you want to use. The release types are; patch (0.0.1), major (0.1.0), or minor (1.0.0).
```
npm version <release_type>
```
This will update the version number in the `package.json`, and will add a git tag automatically. Next you'll need to push the git tag to the remote.
```
git push --tags origin master
```
After that you'll need to publish to npm.
```
npm publish
```

When you're confident with the release, make sure the version tag is also released at GitHub.

## Support

[Frequently Asked Questions](http://dev.flagpack.xyz/support/)

[Documentation](http://dev.flagpack.xyz/docs/)

## Releases

You can find a changelog of Flagpack's releases on the [Releases page](https://github.com/Yummygum/vue-flagpack/releases) on GitHub.

## Contribute

If you're interested in contributing to this project, great! Please see the [contributing document](CONTRIBUTING.md).

## License

Flagpack is an open source project published under a [CC BY 4.0 license](https://creativecommons.org/licenses/by/4.0/).
