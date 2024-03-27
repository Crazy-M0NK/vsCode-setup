# Setup

## Fast setup React Native

```json
{
  "workbench.colorTheme": "Dracula Soft",
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
  "window.zoomLevel": 1,
  "cSpell.userWords": [
    "рэтхолинга",
    "clubpokerspace",
    "esbenp",
    "gradlew",
    "Pressable",
    "rrect",
    "tektur"
  ],
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
    }
  ]
}
```
## Extensios

```shell
code --install-extension aaron-bond.better-comments
code --install-extension alefragnani.project-manager
code --install-extension apollographql.vscode-apollo
code --install-extension bradlc.vscode-tailwindcss
code --install-extension ChakrounAnas.turbo-console-log
code --install-extension christian-kohler.path-intellisense
code --install-extension codezombiech.gitignore
code --install-extension dbaeumer.vscode-eslint
code --install-extension donjayamanne.git-extension-pack
code --install-extension donjayamanne.githistory
code --install-extension DotJoshJohnson.xml
code --install-extension dracula-theme.theme-dracula
code --install-extension dzannotti.vscode-babel-coloring
code --install-extension eamodio.gitlens
code --install-extension esbenp.prettier-vscode
code --install-extension formulahendry.auto-rename-tag
code --install-extension GitHub.copilot
code --install-extension GraphQL.vscode-graphql
code --install-extension GraphQL.vscode-graphql-syntax
code --install-extension Kasik96.swift
code --install-extension kumar-harsh.graphql-for-vscode
code --install-extension lostintangent.vsls-whiteboard
code --install-extension mathiasfrohlich.Kotlin
code --install-extension mikestead.dotenv
code --install-extension ms-vsliveshare.vsliveshare
code --install-extension msjsdiag.vscode-react-native
code --install-extension naumovs.color-highlight
code --install-extension NomicFoundation.hardhat-solidity
code --install-extension Orta.vscode-jest
code --install-extension redhat.vscode-yaml
code --install-extension seunlanlege.action-buttons
code --install-extension sirmspencer.vscode-autohide
code --install-extension spywhere.guides
code --install-extension streetsidesoftware.code-spell-checker
code --install-extension streetsidesoftware.code-spell-checker-russian
code --install-extension TTOOWA.in-your-face-incredible
code --install-extension xabikos.JavaScriptSnippets
code --install-extension ziyasal.vscode-open-in-github
```
