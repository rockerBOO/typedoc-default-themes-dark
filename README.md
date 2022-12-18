# Default themes for TypeDoc with addition of prefers-color-scheme: dark colors

Uses default themes from https://github.com/TypeStrong/typedoc-default-themes with the addition of dark colors for the default theme. 

`@media (prefers-color-scheme: dark)`

See: [src/default/assets/css/_theme.scss](https://github.com/rockerBOO/typedoc-default-themes-dark/blob/dark-theme/src/default/assets/css/_theme.scss)

**Note:** Made for Typedoc < 0.22, as the templating changes in 0.22 to JSX. *No longer supported.* Typedoc seems to support some level of light/dark themes in the defaults. 

## Install

```sh
npm add --dev typedoc-default-themes-dark
```

![screen2](https://gitlab.com/rockerBOO/typedoc-theme-dark/-/raw/master/resources/screen2.png)

![screen3-light](https://gitlab.com/rockerBOO/typedoc-theme-dark/-/raw/master/resources/screen3-light.png)

## Usage

```sh
typedoc ./file.ts --theme ./node_modules/typedoc-default-themes-dark/bin/default/
```

or add the theme to your tsconfig.json
```json
{
  "typedocOptions": {
    "theme": "node_modules/typedoc-default-themes-dark/bin/default/"
  }
}
```

## Build
To make a build:

```sh
npm run build
```

This puts the theme you want to use in `bin/default/`. 


This module contains the default themes of TypeDoc.
Visit https://typedoc.org/ to learn more about TypeDoc.

## Contributing

Contributions are welcome and appreciated. You can find TypeDoc on GitHub, feel free to start
an issue or create a pull requests:<br>
[https://github.com/TypeStrong/typedoc](https://github.com/TypeStrong/typedoc)

To use a local build of this project, run the `npm pack` command in this directory. Then
in the project where you want to use your local build run `npm install ../path/to/typedoc-default-themes-VERSION.tgz`

## License

Copyright (c) 2015 [Sebastian Lenz](http://www.sebastian-lenz.de).<br>
Copyright (c) 2016-2020 [TypeDoc Contributors](https://github.com/TypeStrong/typedoc/graphs/contributors).<br>
Licensed under the Apache License 2.0.
