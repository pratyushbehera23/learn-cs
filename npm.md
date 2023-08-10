# npm

Package manager for node.js
Install Node.js, npm comes along with it
Other package manager for node: pnpm yarn

<!-- Some packages:
chalk
tailwind
Vue Webpack Snowpack
Sass Gulp Postcss
-->

## Install packages

### Global install

Most packages should be installed locally
Some packages need to installed globally to access from any directory in your computer.

```sh
npm install -g packagename
```

### Local install

Gets installed inside project folder

```sh
npm install packagename
```

package.json
package-lock.json

```sh
npm init
npm init -y
```

```sh
npm i
```

node_modules

```sh
npm list
```

## Package versioning & updating

major.minor.patch

Major - big changes; not backwards-compatible
Minor - backwards-compatible
Patch - small bug fixes

1.0.0 - first public release

```sh
npm view packagename versions
npm update packagename
```
