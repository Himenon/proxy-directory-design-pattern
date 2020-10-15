# @himenon/proxy-directory-design-pattern


An example where the library supports cjs and esm, but provides a single module format for the user.

|Registry|Status|
|:-------|:-----|
|GitHub|[![GitHub version](https://badge.fury.io/gh/Himenon%2Fproxy-directory-design-pattern.svg)](https://badge.fury.io/gh/Himenon%2Fproxy-directory-design-pattern)|
|npm|[![npm version](https://badge.fury.io/js/%40himenon%2Fproxy-directory-design-pattern.svg)](https://badge.fury.io/js/%40himenon%2Fproxy-directory-design-pattern)|

## Usage

```bash
yarn add @himenon/proxy-directory-design-pattern
```

### All import

```ts
import * as Lib from "@himenon/proxy-directory-design-pattern";

Lib.PackageA.exec();
Lib.PackageB.exec();
```

### Individual import

```ts
import * as PackageA from "@himenon/proxy-directory-design-pattern/PackageA";
import * as PackageB from "@himenon/proxy-directory-design-pattern/PackageB";

PackageA.exec();
PackageB.exec();
```

## Development

### Release

release version

```bash
yarn run lerna version --yes
```

### Revert release (before execute GitHub Actions)

reset version

```bash
git tag -d [tag]
git push origin :[tag]
```

## Reference

* https://www.npmjs.com/package/cherry-pick
* https://developers.livechat.com/updates/how-to-create-javascript-libraries-in-2018-part-2#proxy-directories

## LICENSE

@himenon/proxy-directory-design-pattern is [MIT licensed](./LICENSE).
