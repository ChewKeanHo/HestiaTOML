# Hestia Libraries - `HestiaTOML`

[![Hestia Libraries](https://raw.githubusercontent.com/ChewKeanHo/hestiaTOML/main/src/icons/banner_1200x270.svg)](#)

One Peaceful Frontend+Backend Software Library Suite.

This repository facilitates
[Tom's Obvious Minimal Language](https://github.com/toml-lang/toml) operation
for all Hestia Libraries user. This library uses the character-based
streaming with low memory and low footprint (e.g.
microcontroller adata processing) considerations.




## Why It Matters

This project was initiated primarily because of:

1. **Ensures proper interoperability between programming languages** -
   making sure the `hestiaTOML` library talks to each other seamlessly across
   programming languages with the same context.
2. **Friendly to low memory and low footprint environment** - using simple
   string character streaming algorithm to parse the required data from TOML
   syntax.
3. **Consumption freedom** - HestiaTOML makes NO decision and NO assumption on
   how you consume the parsed data: use the corresponding data type sanitization
   function to convert from `string` into your desired data type, not here.
5. **Simple to integrate** - simple enough to use for all supported programming
   languages.




## Design Principles

The definitions complies to only the following rules:

1. **STRICTLY**: **Everthing is a `string`**.
2. Primarily uses Unicode for internal operations.
3. Uses syntax behaviorial table algorithm even for restrictive languages like
   POSIX Shell (not BASH).

This library is heavily guarded with unit tests whenever available.




## Setup

This library supports multiple programming languages for the same dataset.
Please import based on your programming language(s) using the instructions in
the sub-sections below.

Please do note that branches like `main`, `next`, and `experimental` are for
maintenance & development uses (as in, the production factory itself). Hence,
please avoid them and only use it at your own risk.



### Javascript|Typescript Ecosystems

To use `hestiaTOML` library in your Javascript|Typescript project, you may use
the following methods for integrations:


#### Git Release Branches (Recommended)

It's highly recommended to use `git` release branches inside your `package.json`
dependencies list. This is to avoid the registry configurations problem
involving `npm`:

```
{
  "dependencies": {
    ...
    "@chewkeanho/hestiaSTRING": "git+https://github.com/ChewKeanHo/hestiaSTRING.git#[VERSION]_npm",
    ...
    "@chewkeanho/hestiaTOML": "git+https://github.com/ChewKeanHo/hestiaTOML.git#[VERSION]_npm"
    ...
  }
}
```

For always latest release, please use the `latest` version tag. Example:

```
{
  ...
  "dependencies": {
    ...
    "@chewkeanho/hestiaSTRING": "git+https://github.com/ChewKeanHo/hestiaSTRING.git#[VERSION]_npm",
    ...
    "@chewkeanho/hestiaTOML": "git+https://github.com/ChewKeanHo/hestiaTOML.git#latest_npm"
    ...
  }
  ...
}
```


#### NPM

> **NOTE**
>
> To be updated.




## Data Source

The libraries are based on the following data sources:

1. Specification - https://github.com/toml-lang/toml




## License

This project is licensed under [OSI compliant Apache 2.0 License](LICENSE.txt).
