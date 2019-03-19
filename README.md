# umi-lib-namedExports-problem

## 重现

Build package 正常。

```bash
$ cd package
$ yarn
$ yarn run build
```

Build lerna 不正常。

```bash
$ cd lerna/packages/foo
$ yarn
$ cd ../../
$ yarn run build
```

报错如下：

```bash
Error: 'default' is not exported by packages/foo/node_modules/timing2/lib/index.js
```
