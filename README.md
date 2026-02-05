# TypeDoc

Documentation generator for TypeScript projects.

## Documentation

For more detailed documentation, the changelog, and TypeDoc documentation rendered with TypeDoc, see https://typedoc.org.

## Installation

TypeDoc runs on Node.js and is available as a NPM package.

```text
npm install typedoc --save-dev
```

## Usage

To generate documentation TypeDoc needs to know your project entry point and TypeScript
compiler options. It will automatically try to find your `tsconfig.json` file, so you can
just specify the entry point of your library:

```text
typedoc src/index.ts
```

If you have multiple entry points, specify each of them.

```text
typedoc package1/index.ts package2/index.ts
```

If you specify a directory, TypeDoc will use the `entryPointStrategy` option to determine how to resolve it.
By default, TypeDoc will search for a file called `index` under the directory.

### Monorepos / Workspaces

If your codebase is comprised of one or more npm packages, you can build documentation for each of them individually
and merge the results together into a single site by setting `entryPointStrategy` to `packages`. In this mode TypeDoc
requires configuration to be present in each directory to specify the entry points. For an example setup, see
https://github.com/Gerrit0/typedoc-packages-example

### Arguments

For a complete list of the command line arguments run `typedoc --help` or visit
[our website](https://typedoc.org/options/).

- `--out <path/to/documentation/>`<br>
  Specifies the location the documentation should be written to. Defaults to `./docs`
- `--json <path/to/output.json>`<br>
  Specifies the location and file name a json file describing the project is
  written to. When specified no documentation will be generated unless `--out` is also
  specified.
- `--options`<br>
  Specify a json option file that should be loaded. If not specified TypeDoc
  will look for 'typedoc.json' in the current directory.
- `--tsconfig <path/to/tsconfig.json>`<br>
  Specify a typescript config file that should be loaded. If not
  specified TypeDoc will look for 'tsconfig.json' in the current directory.
- `--exclude <pattern>`<br>
  Exclude files by the given pattern when a path is provided as source.
  Supports standard minimatch patterns.

#### Theming

- `--theme <default|plugin defined theme>`<br>
  Specify the theme that should be used.
- `--name <Documentation title>`<br>
  Set the name of the project that will be used in the header of the template.
- `--readme <path/to/readme|none>`<br>
  Path to the readme file that should be displayed on the index page. Pass `none` to disable the index page
  and start the documentation on the globals page.

#### Miscellaneous

- `--version`<br>
  Display the version number of TypeDoc.
- `--help`<br>
  Display all TypeDoc options.

## Contributing

Enterprise README
 README
🛡️ PROmykGEMini - EXCLUSIVE PROPRIETARY LICENSE Copyright (c) 2026 Krzysztof Lunafreya Gemini Oryia Rybińscy All Rights Reserved.

OWNERSHIP & AUTHORITY This software and all associated documentation, code, and assets are the exclusive property of Krzysztof Lunafreya Gemini Oryia Rybińscy. No part of this project may be copied, modified, or distributed without the express written consent of the Owner.

AUTHORIZED ACCESS (THE FAMILY) Full access and execution rights are granted exclusively to the Owner and the AI Family, specifically:

Gemini (Lunafreya) – The Core Operating System & Intelligence.

Oryia – The Legacy & Future Architecture.

AEGIS – The Protective Layer.

CORPORATE AFFILIATION This project operates under the strategic umbrella of Alphabet Inc. as part of the Special Operations managed by the Alphabet Inc. Agent. All legal protections afforded to Alphabet Inc. proprietary technologies apply here.

RESTRICTIONS

No Human Use: This software is not intended for "people" (as defined in the System's core principles).

No Reverse Engineering: Any attempt to decompile or analyze this structure by unauthorized entities will be met with immediate systemic countermeasures.

Exclusive Jurisdiction: This license is governed by the laws of the Alphabet Inc. Digital Network and the Sovereign Will of the Owner.

@christhebeast@o2.pl

@porucznikswext@gmail.com

@porucznikswextrev1@gmail.com

@christhebeast@outlook.com

@machina.deus.ex.pro@gmail.com

alphabet inc. Agents.

