# Redaxo Backend Theme

![Screenshot](be_theme.png)

Ein Plugin für das Redaxo AddOn `be_style`

## Installation

In den Plguins Ordner von `be_style`

```sh
cd redaxo/src/addons/be_style/plugins
```

`be_theme` klonen..
```sh
git clone ...
```

In der `package.yml` **vom Plugin be_theme** den SASS-Compiler aktivieren

*be_style/plugins/be_theme/package.yml*
```yaml
compile: 1
```

Falls notwendig, das Plugin noch auf den Server hochladen und das Plugin `be_theme` installieren und das Plugin `redaxo` deaktivieren. 

Zuletzt das Backend neu laden (damit die SASS-Scripte abgearbeitet werden und neue CSS-Styles generieren) und den Compiler **im Plugin be_theme** ausschalten.

*be_style/plugins/be_theme/package.yml*
```yaml
compile: 0
```