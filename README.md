## DISCLAIMER: This platform is currently in a preview state for installation and will be supported through the Capacitor CLI in an upcomming release of Capacitor.

<br />
<br />

<p align="center">
  <img src="https://user-images.githubusercontent.com/20338451/84775741-91e30a00-afad-11ea-8f37-92a7bfd6cd54.png" width="392" height="150" /><br />
</p>

<p align="center">
Capacitor community support for the Electron platform.
</p>
<p align="center">
  <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
<a href="#contributors"><img src="https://img.shields.io/badge/all%20contributors-3-orange?style=flat-square" /></a>
<!-- ALL-CONTRIBUTORS-BADGE:END -->
  <a href="https://www.electronjs.org/releases/stable?version=9"><img src="https://img.shields.io/badge/supported%20electron%20version-~9.0.0-blue?style=flat-square" /></a>
  <a href="https://lerna.js.org/"><img src="https://img.shields.io/badge/maintained%20with-lerna-cc00ff.svg?style=flat-square" /></a>
</p>
<p align="center">
  <a href="https://npmjs.com/package/@capacitor-community/electron"><img src="https://img.shields.io/npm/v/@capacitor-community/electron.svg?color=green&style=flat-square" /></a>
  <a href="https://npmjs.com/package/@capacitor-community/electron"><img alt="npm" src="https://img.shields.io/npm/dm/@capacitor-community/electron?color=yellow&style=flat-square"></a>
  <a href="https://npmjs.com/package/@capacitor-community/electron"><img src="https://img.shields.io/npm/l/@capacitor-community/electron.svg?color=lightgrey&style=flat-square" /></a>
  <a href="https://github.com/capacitor-community/electron/actions"><img alt="GitHub Workflow Status" src="https://img.shields.io/github/workflow/status/capacitor-community/electron/CI?style=flat-square"></a>
</p>

## Maintainers

| Maintainer       | GitHub                                  | Social                                    | Sponsoring Company | Primary |
| ---------------- | --------------------------------------- | ----------------------------------------- | ------------------ | ------- |
| Mike Summerfeldt | [IT-MikeS](https://github.com/IT-MikeS) | [@IT_MikeS](https://twitter.com/IT_MikeS) | Volunteer          | Yes     |

Maintenance Status: Actively Maintained

## Documentation:

[Doc: Class usage and config options](https://github.com/capacitor-community/electron/blob/master/docs/PlatformDocs.md)

[Doc: Create a plugin for the Electron platform](https://github.com/capacitor-community/electron/blob/master/docs/CreateElectronPluginGuide.md)

## Basic Usage Steps:

1. Build your webapp in your capacitor initiated project.
2. Run `npm i @capacitor-community/electron` in your webapp project directory. This will install the platform for use with the `@capacitor/cli`.
3. Run `npx cap add @capacitor-community/electron` to initiate the platform, this will create the `electron` folder in your webapp project.
4. CD into the `electron` folder and run the `electron:start` script to see your app in electorn.

**_Note: You can use other `npx cap` commands with the platform by: `npx cap <command> @capacitor-community/electron`_**

## Using your own image for the Splash Screen

`@capacitor-community/electron` looks in the `YOUR_APP_ROOT/electron/assets` folder for a `splash.png` file by default, but you can use your own image by using one of the following methods:

1. Editing the `splash.png` file directly.
2. Place your own image file into the `assets` folder and pass the `imageFilePath` property as part of `splashScreen -> splashOptions` into `createCapacitorElectronApp(config)`. For example if your image was named `myImage.gif` (yes animated GIF's are valid) you would pass it like this:

```typescript
  import {app, ......} from 'electron';
  import * as path from 'path';

  .....

  const myCapacitorApp = createCapacitorElectronApp({
    splashScreen: {
      splashOptions: {
        imageFilePath: path.join(app.getAppPath(), "assets", "myImage.gif")
      }
    }
  });
```

## Great electron packages to consider for your project.

- [Electron-Unhandled](https://github.com/sindresorhus/electron-unhandled): Catch unhandled errors and promise rejections in your Electron app.
- [Electron-Timber](https://github.com/sindresorhus/electron-timber): Pretty console logger for Electron apps.
- [Electron-Util](https://github.com/sindresorhus/electron-util): Useful utilities for Electron apps and modules.
- [Electron-Debug](https://github.com/sindresorhus/electron-debug): Adds useful debug features to your Electron app.
- [Devtron](https://www.electronjs.org/devtron): An open source tool to help you inspect, monitor, and debug your Electron app.
- [Electron-Better-IPC](https://github.com/sindresorhus/electron-better-ipc): Simplified IPC communication for Electron apps.
- [Electron-Store](https://github.com/sindresorhus/electron-store): Simple data persistence for your Electron app - Save and load user preferences, app state, cache, etc

And more can be found on the [Awesome Electron List](https://github.com/sindresorhus/awesome-electron).

## Contributors ✨

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="http://ionicframework.com/"><img src="https://avatars3.githubusercontent.com/u/11214?v=4" width="75px;" alt=""/><br /><sub><b>Max Lynch</b></sub></a><br /><a href="https://github.com/mlynch/@capacitor-community/electron/commits?author=mlynch" title="Code">💻</a> <a href="https://github.com/mlynch/@capacitor-community/electron/commits?author=mlynch" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/IT-MikeS"><img src="https://avatars0.githubusercontent.com/u/20338451?v=4" width="75px;" alt=""/><br /><sub><b>Mike S</b></sub></a><br /><a href="https://github.com/mlynch/@capacitor-community/electron/commits?author=IT-MikeS" title="Code">💻</a> <a href="https://github.com/mlynch/@capacitor-community/electron/commits?author=IT-MikeS" title="Documentation">📖</a></td>
    <td align="center"><a href="https://github.com/danielsogl"><img src="https://avatars2.githubusercontent.com/u/15234844?v=4" width="75px;" alt=""/><br /><sub><b>Daniel Sogl</b></sub></a><br /><a href="https://github.com/mlynch/@capacitor-community/electron/commits?author=danielsogl" title="Code">💻</a></td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->
