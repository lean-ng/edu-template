# Project: edu-template

> Template-Repository für meine Schulungsbeispiele

Das Projekt wurde ursprünglich generiert mit der [Angular CLI](https://github.com/angular/angular-cli) (Version 12.2.10).

## Bootstrap Integration

- Installiere Bootstrap

  `npm install bootstrap`

- Styles importieren über den Weg [Precompiled Sass](https://getbootstrap.com/docs/5.1/getting-started/webpack/#importing-styles)

  - Globale Styles verschieben nach `./src/scss/styles.scss`. Der Ordner `scss` ist natürlich frei gewählt. Hätte man auch einfach als `./src/styles.scss` nur umbennen können.
  - In der `./angular.json` den Pfad anpassen (in der `build`- und in der `test`-Konfiguration)
  - In der `./angular.json` die Component-Schematics auf `scss`-Styles umstellen.

- Bootstrap in der globalen `styles.scss` importieren und ein Custom-Stylesheet `./src/scss/_custom.scss` anlegen:

  ```scss
  @import 'custom';
  @import '~bootstrap/scss/bootstrap';`
  ```

## Features

- Node-Version: LTS wird eingestellt für nvm-Nutzer (Datei `.nvmrc`)
- Code Linting via ESLint (siehe [Angular ESLint](https://github.com/angular-eslint/angular-eslint))
- Code Formatting via Prettier

## VS Code Extensions

- Angular Language Service
- EditorConfig
- ESLint
- Prettier

## VS Code Settings

- Format on Save
