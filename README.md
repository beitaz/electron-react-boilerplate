# 纯纯饰品

## Install

- [错误指导](https://github.com/electron-react-boilerplate/electron-react-boilerplate/issues/400)\*\*

First, clone the repo via git:

```bash
$ git clone --depth 1 --single-branch --branch master https://github.com/electron-react-boilerplate/electron-react-boilerplate.git cc
$ cd your-project-name
$ npm config set registry 'https://registry.npm.taobao.org'
$ ELECTRON_MIRROR=http://npm.taobao.org/mirrors/electron/ npm install -g electron@2.0.14
$ SASS_BINARY_SITE=http://npm.taobao.org/mirrors/node-sass npm install -g node-sass
$ npm install -g phantomjs --phantomjs_cdnurl=http://npm.taobao.org/mirrors/phantomjs
$ npm install -g chromedriver --chromedriver_cdnurl=http://npm.taobao.org/mirrors/chromedriver
$ npm link electron node-sass chromedriver phantomjs
$ npm install
$ yarn
...
```

**无法下载 `node ./download-chromedriver.js` 这个问题必须解决.**

> On my Mac I deleted all folders with the prefix electron under /Users/**`username`**/.npm

## 开发

如果不需要自动重启服务,执行以下命令时带上 `START_MINIMIZED=true` 即可:

```bash
$ [START_MINIMIZED=true] yarn dev
...
```

_提示_ 此命令等效于同时执行 `yarn start-renderer-dev` 和 `yarn start-main-dev` 命令.

## 打包发布

```bash
$ yarn package
...
```

_提示_ 此命令默认打包为当前平台.其他可用脚本: `package-ci`(Travis CI), `package-linux`(Linux), `package-win`(Windows) 和 `package-all` 全平台.

## 参考信息

- [Run commands concurrently](https://github.com/kimmobrunfeldt/concurrently) 同时运行多个命令.
- [Cross platform setting of environment scripts](https://github.com/kentcdodds/cross-env) 设置跨平台的脚本环境
- [Prettier is an opinionated code formatter](https://github.com/prettier/prettier) 代码格式化
- [Run linters on git staged files](https://github.com/okonet/lint-staged) Git staged 代码检查

## 特别致谢

- [ElectronReact](https://electron-react-boilerplate.js.org/docs/en/installation)

[npm-image]: https://img.shields.io/npm/v/electron-react-boilerplate.svg?style=flat-square
[github-tag-image]: https://img.shields.io/github/tag/electron-react-boilerplate/electron-react-boilerplate.svg
[github-tag-url]: https://github.com/electron-react-boilerplate/electron-react-boilerplate/releases/latest
[travis-image]: https://travis-ci.com/electron-react-boilerplate/electron-react-boilerplate.svg?branch=master
[travis-url]: https://travis-ci.com/electron-react-boilerplate/electron-react-boilerplate
[appveyor-image]: https://ci.appveyor.com/api/projects/status/github/electron-react-boilerplate/electron-react-boilerplate?svg=true
[appveyor-url]: https://ci.appveyor.com/project/electron-react-boilerplate/electron-react-boilerplate/branch/master
[david_img]: https://img.shields.io/david/electron-react-boilerplate/electron-react-boilerplate.svg
[david_site]: https://david-dm.org/electron-react-boilerplate/electron-react-boilerplate
[david_img_dev]: https://david-dm.org/electron-react-boilerplate/electron-react-boilerplate/dev-status.svg
[david_site_dev]: https://david-dm.org/electron-react-boilerplate/electron-react-boilerplate?type=dev
