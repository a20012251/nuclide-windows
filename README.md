# Developing Nuclide on Windows

## vim-mode-plus

On your global keymap make sure to add

```
'atom-text-editor.vim-mode-plus.normal-mode':
  'ctrl-t': 'unset!'
```

## flow

Make sure to run `npm install -g flow-bin@version`, where `version` is the version in the last line of the .flowconfig file in the root of the nuclide tree.

## temporary workaround for flow errors

Put this in the ignore part of your .flowconfig

```
<PROJECT_ROOT>/node_modules/eslint-plugin-jsx-a11y/.*
<PROJECT_ROOT>/node_modules/graphql-language-service-interface/.*
<PROJECT_ROOT>/node_modules/graphql-language-service-parser/.*
<PROJECT_ROOT>/node_modules/graphql-language-service-types/.*
<PROJECT_ROOT>/node_modules/graphql-language-service-server/.*
<PROJECT_ROOT>/node_modules/graphql-language-service-utils/.*
<PROJECT_ROOT>/node_modules/graphql-language-service/.*
<PROJECT_ROOT>/node_modules/graphql/.*
```
