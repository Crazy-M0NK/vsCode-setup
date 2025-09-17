# Fast setup Visual Studio Code (React/React Native)

## settings.json
path: {any path to vscode}/Code/User

```json
{
  "workbench.colorTheme": "Dracula Theme Soft",
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.formatOnSave": true,
  "editor.suggestSelection": "first",
  "editor.formatOnPaste": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": "explicit"
  },
  "turboConsoleLog.addSemicolonInTheEnd": true,
  "turboConsoleLog.delimiterInsideMessage": "-",
  "turboConsoleLog.includeFileNameAndLineNum": false,
  "turboConsoleLog.insertEnclosingClass": false,
  "turboConsoleLog.insertEnclosingFunction": false,
  "turboConsoleLog.logMessagePrefix": "🚀",
  "turboConsoleLog.quote": "'",
  "guides.normal.width": 0.8,
  "cSpell.language": "en,ru-RU,en-GB,en-US",
  "actionButtons": {
    "defaultColor": "#ff0034", // Can also use string color names.
    "loadNpmCommands": false, // Disables automatic generation of actions for npm commands.
    "reloadButton": "♻️", // Custom reload button text or icon (default ↻). null value enables automatic reload on configuration change
  //Only for Raect-Native
    "commands": [
      {
        "name": "Ⓜ️ Run metro (no-cache)",
        "color": "#176cff",
        "command": "yarn start"
      },
      {
        "name": "📱 run android",
        "color": "#4FAF53",
        "singleInstance": true,
        "command": "yarn android" // This is executed in the terminal.
      },
      {
        "name": "💠 Run Metro (Full Clear Cache)",
        "color": "#25C7ED",
        "command": "rm -f yarn.lock && cd android && ./gradlew clean && cd .. && yarn && yarn start"
      },
      {
        "name": "📲 Release build ",
        "color": "#ffcd17",
        "command": "yarn android-build"
      }
    ]
  },
  "editor.minimap.enabled": false,
  "editor.inlineSuggest.enabled": true,
  "typescript.updateImportsOnFileMove.enabled": "always",
  "git.openRepositoryInParentFolders": "never",
  "git.enableSmartCommit": true,
  "git.confirmSync": false,
  "gitlens.graph.layout": "editor",
  "gitlens.graph.minimap.enabled": false,
  "explorer.confirmDelete": false,
  "javascript.updateImportsOnFileMove.enabled": "always",
  "explorer.confirmDragAndDrop": false,
  "react-native-tools.showUserTips": false,
  "window.zoomLevel": 0.5,
  "extensions.ignoreRecommendations": true,
  "gitlens.advanced.messages": {
    "suppressCreatePullRequestPrompt": true
  },
  "workbench.settings.applyToAllProfiles": [],
  "better-comments.tags": [
    {
      "tag": "!",
      "color": "#FF2D00",
      "strikethrough": false,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": false,
      "italic": false
    },
    {
      "tag": "?",
      "color": "#3498DB",
      "strikethrough": false,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": false,
      "italic": false
    },
    {
      "tag": "//",
      "color": "#474747",
      "strikethrough": true,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": false,
      "italic": false
    },
    {
      "tag": "TODO",
      "color": "#FF8C00",
      "strikethrough": false,
      "underline": false,
      "backgroundColor": "black",
      "bold": false,
      "italic": false
    },
    {
      "tag": "*",
      "color": "#98C379",
      "strikethrough": false,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": false,
      "italic": false
    },
    {
      "tag": ">",
      "color": "#990FBE",
      "strikethrough": false,
      "underline": false,
      "backgroundColor": "transparent",
      "bold": false,
      "italic": false
    }
  ],
  "git.autofetch": true,
  "gitlens.launchpad.indicator.polling.interval": 15,
  "gitlens.launchpad.indicator.useColors": true,
  "gitlens.graph.layout": "editor",
  "diffEditor.ignoreTrimWhitespace": false,
  "eslint.codeActionsOnSave.rules": null,
  "eslint.execArgv": null,
  "eslint.workingDirectories": [],
  "window.customTitleBarVisibility": "auto",
  "window.commandCenter": false,
  "workbench.layoutControl.enabled": false,
  "workbench.editorAssociations": {
    "{git,gitlens}:/**/*.{md,csv,svg}": "default",
    "*.svg": "default"
  },
  "explorer.confirmPasteNative": false,
  "[xml]": {
    "editor.defaultFormatter": "DotJoshJohnson.xml"
  },
  "python.defaultInterpreterPath": "/bin/python3.12",
  "tailwindCSS.includeLanguages": {
    "css": "css",
    "postcss": "css",
    "scss": "css",
    "javascript": "javascript",
    "javascriptreact": "javascript",
    "typescript": "typescript",
    "typescriptreact": "typescript"
  }
}
```
## Extensios

```shell

ext install aaron-bond.better-comments
ext install chakrounanas.turbo-console-log
ext install christian-kohler.path-intellisense
ext install codezombiech.gitignore
ext install dbaeumer.vscode-eslint
ext install donjayamanne.git-extension-pack
ext install dotjoshjohnson.xml
ext install dracula-theme.theme-dracula
ext install dzannotti.vscode-babel-coloring
ext install eamodio.gitlens
ext install esbenp.prettier-vscode
ext install mathiasfrohlich.kotlin
ext install mikestead.dotenv
ext install ms-azuretools.vscode-docker
ext install ms-python.debugpy
ext install ms-python.python
ext install ms-python.vscode-python-envs
ext install ms-python.vscode-pylance
ext install msjsdiag.vscode-react-native
ext install naumovs.color-highlight
ext install redhat.java
ext install redhat.vscode-yaml
ext install seunlanlege.action-buttons
ext install simonsiefke.svg-preview
ext install bradlc.vscode-tailwindcss
ext install spywhere.guides
ext install streetsidesoftware.code-spell-checker
ext install streetsidesoftware.code-spell-checker-russian
ext install visualstudioexptteam.intellicode-api-usage-examples
ext install visualstudioexptteam.vscodeintellicode
ext install vscjava.vscode-gradle
ext install vscjava.vscode-java-dependency
ext install vscjava.vscode-java-pack
ext install vscjava.vscode-maven
ext install xabikos.javascriptsnippets
ext install ziyasal.vscode-open-in-github
ext install ms-azuretools.vscode-containers
ext install mhutchie.git-graph
```
# App init

## .eslintrc.json

```json
{
  "root": true,
  "extends": ["@react-native-community", "prettier"],
  "parser": "@typescript-eslint/parser",
  "plugins": ["react", "react-hooks", "import"],
  "overrides": [
    {
      "files": ["*.ts", "*.tsx", "*.js", "*.jsx"],
      "env": {
        "jest": true
      },
      "rules": {
        "no-param-reassign": 0,
        "react/react-in-jsx-scope": "off",
        "import/order": [
          "error",
          {
            "groups": ["builtin", "external", "internal", "sibling"],
            "pathGroups": [
              {
                "pattern": "react",
                "group": "builtin",
                "position": "before"
              },
              {
                "pattern": "src/**",
                "group": "external",
                "position": "after"
              }
            ],
            "pathGroupsExcludedImportTypes": ["react"],
            "newlines-between": "always",
            "alphabetize": {
              "order": "asc",
              "caseInsensitive": true
            }
          }
        ],
        "sort-imports": [
          "error",
          {
            "ignoreDeclarationSort": true
          }
        ],
        "import/no-default-export": 0,
        "react-native/no-unused-styles": 0,
        "react-native/no-inline-styles": 2,
        "react-native/no-color-literals": 2,
        "import/prefer-default-export": 0,
        "@typescript-eslint/naming-convention": [
          "error",
          {
            "selector": "variable",
            "format": ["camelCase", "UPPER_CASE", "PascalCase", "snake_case"]
          }
        ]
      }
    }
  ],
  "rules": {
    "global-require": 0,
    "no-param-reassign": [
      2,
      {"props": true, "ignorePropertyModificationsForRegex": ["^acc"]}
    ],
    "react-hooks/rules-of-hooks": "error",
    "react-hooks/exhaustive-deps": "warn",
    "react/function-component-definition": [
      1,
      {"namedComponents": "function-declaration"}
    ],
    "@typescript-eslint/no-unused-vars": "error",
    "@typescript-eslint/no-explicit-any": "error",
    "import/prefer-default-export": 1
  }
}
```
## .prettierrc.js

```js
module.exports = {
  arrowParens: 'avoid',
  bracketSameLine: true,
  bracketSpacing: false,
  singleQuote: true,
  trailingComma: 'all',
  printWidth: 90,
};
```
## tsconfig.json

```json
{
  "extends": "@react-native/typescript-config/tsconfig.json",
  "module": "es2020", // ensures output is ESM
  "target": "es2020",
  "include": ["src/**/*"],
  "compilerOptions": {
    /* Visit https://aka.ms/tsconfig.json to read more about this file */
    "baseUrl": ".",
    "paths": {
      "src/*": ["src/*"]
    },
    "noImplicitAny": false,
    /* Completeness */
    "skipLibCheck": true /* Skip type checking all .d.ts files. */
  }
}
```
## react-native.config.js

```js
module.exports = {
  project: {
    ios: {},
    android: {},
  },
  assets: ['./src/assets/fonts/'],
};
```
## babel.config.js

```js
module.exports = {
  presets: ['module:@react-native/babel-preset'],
  plugins: [
    [
      'module-resolver',
      {
        alias: {
          src: './src',
        },
      },
    ],
    [
      'module:react-native-dotenv',
      {
        envName: 'APP_ENV',
        moduleName: '@env',
        path: '.env',
        safe: false,
        allowUndefined: true,
        verbose: false,
      },
    ],
    'react-native-reanimated/plugin',
  ],
};
```
## jest.setup.js

```js
//? Need to figure this out
import mockRNDeviceInfo from 'react-native-device-info/jest/react-native-device-info-mock';
import mockSafeAreaContext from 'react-native-safe-area-context/jest/mock';

// Note: test renderer must be required after react-native.
jest.useFakeTimers();
jest.mock('@react-native-async-storage/async-storage', () =>
  require('@react-native-async-storage/async-storage/jest/async-storage-mock'),
);
jest.useFakeTimers();
jest.mock('react-native-device-info', () => mockRNDeviceInfo);
jest.mock('react-native-localize', () => {
  return {
    getLocales: () => [{languageCode: 'en'}],
    // you can add other functions mock here that you are using
  };
});

jest.mock('react-native', () => {
  const RN = jest.requireActual('react-native');

  RN.NativeModules.SettingsManager = {
    settings: {
      AppleLocale: 'en-US',
      AppleLanguages: ['fr-FR', 'en-US'],
    },
  };
  return RN;
});

jest.mock('react-i18next', () => ({
  // this mock makes sure any components using the translate hook can use it without a warning being shown
  initReactI18next: {type: '3rdParty', init: jest.fn()},
  useTranslation: () => {
    return {
      t: str => str,
      i18n: {
        changeLanguage: () => new Promise(() => {}),
      },
    };
  },
}));
jest.mock('react-native/Libraries/EventEmitter/NativeEventEmitter');
jest.mock('react-native-safe-area-context', () => mockSafeAreaContext);

jest.mock('react-native-keychain', () => {
  return {
    setGenericPassword: jest.fn(),
    getGenericPassword: jest.fn(),
    getInternetCredentials: jest.fn(),
    setInternetCredentials: jest.fn(),
  };
});
export const mockedNavigate = jest.fn();
jest.mock('@react-navigation/native', () => {
  const actualNav = jest.requireActual('@react-navigation/native');
  return {
    ...actualNav,
    useNavigation: () => ({
      navigate: mockedNavigate,
      dispatch: jest.fn(),
    }),
    useIsFocused: () => jest.fn(),
  };
});
```
## package.json

```json
{
  "scripts": {
    "android": "react-native run-android --active-arch-only",
    "ios": "react-native run-ios",
    "ios:14": "react-native run-ios --simulator='iPhone 14'",
    "ios:13-mini": "react-native run-ios --simulator='iPhone 13 mini (16.0)'",
    "cdpi": "cd ios && pod install",
    "lint": "eslint .",
    "start": "react-native start --reset-cache",
    "test": "jest src/*",
    "link-asset": "npx react-native-asset",
    "postinstall": "patch-package",
    "android-build": "cd android && chmod +x gradlew && ./gradlew assembleRelease"
  },
}
```

## Install packages

```
yarn add -D babel-plugin-module-resolver eslint-plugin-import eslint-plugin-react eslint-plugin-react-hooks prettier eslint @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint-plugin-react eslint-plugin-react-hooks
```
### [Skia](https://shopify.github.io/react-native-skia/docs/getting-started/installation)
### [Safe Area Context](https://github.com/th3rdwave/react-native-safe-area-context)
### [Reanimated](https://docs.swmansion.com/react-native-reanimated/docs/fundamentals/getting-started/)
### [DotEnv](https://github.com/goatandsheep/react-native-dotenv)
### [React Navigation](https://reactnavigation.org/docs/getting-started/)
### [Remove console logs in production](https://reactnative.dev/docs/performance#using-consolelog-statements)
