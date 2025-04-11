# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.26.2](https://github.com/Rawk/rasn/compare/rasn-derive-v0.26.1...rasn-derive-v0.26.2) - 2025-04-11

### Added

- support multi-field tuple-structs with delegate if other types are ([#436](https://github.com/Rawk/rasn/pull/436))

### Fixed

- improve constraint performance and bounded intersection ([#440](https://github.com/Rawk/rasn/pull/440))

## [0.22.2](https://github.com/librasn/rasn/compare/rasn-derive-v0.22.1...rasn-derive-v0.22.2) - 2025-01-05

### Other

- Better error messages for derives ([#400](https://github.com/librasn/rasn/pull/400))

## [0.21.0](https://github.com/librasn/rasn/compare/rasn-derive-v0.20.2...rasn-derive-v0.21.0) - 2024-11-12

### Fixed

- cleanup some unnecessary dependencies ([#362](https://github.com/librasn/rasn/pull/362))
- Don't override generics impl in proc-macros on encode impl ([#354](https://github.com/librasn/rasn/pull/354))
- decoding of extended fields in sequence in BER ([#351](https://github.com/librasn/rasn/pull/351))

### Other

- Extract proc macro into own crate ([#364](https://github.com/librasn/rasn/pull/364))
- Optimize field presence tracking of default/optional/extended fields ([#324](https://github.com/librasn/rasn/pull/324))
- Disallow structs without fields for a `set` ([#352](https://github.com/librasn/rasn/pull/352))
- update dependencies

## [0.20.2](https://github.com/librasn/rasn/compare/rasn-derive-v0.20.1...rasn-derive-v0.20.2) - 2024-10-18

### Fixed

- Run clippy and rustdoc only on stable channel in CI ([#342](https://github.com/librasn/rasn/pull/342))

### Other

- Update to syn2 ([#345](https://github.com/librasn/rasn/pull/345))

## [0.19.0](https://github.com/librasn/rasn/compare/rasn-derive-v0.18.0...rasn-derive-v0.19.0) - 2024-09-22

### Other

- clippy fixes

## [0.18.0](https://github.com/librasn/rasn/compare/rasn-derive-v0.17.3...rasn-derive-v0.18.0) - 2024-09-17

### Added

- [**breaking**] Remove option_type ([#329](https://github.com/librasn/rasn/pull/329))
- Constraint utilities, const default, more const functions ([#321](https://github.com/librasn/rasn/pull/321))

### Fixed

- macros: include license texts in the packaged crate ([#330](https://github.com/librasn/rasn/pull/330))
- [**breaking**] Remove Tag and TagTree from module root

## [0.17.3](https://github.com/librasn/rasn/compare/rasn-derive-v0.17.2...rasn-derive-v0.17.3) - 2024-09-12

### Other

- Update itertools to 0.13, update Cargo.lock

## [0.16.0](https://github.com/librasn/rasn/compare/rasn-derive-v0.15.3...rasn-derive-v0.16.0) - 2024-07-17

### Other
- Fix error name regression introduced in a75b26b ([#285](https://github.com/librasn/rasn/pull/285))

## [0.15.3](https://github.com/librasn/rasn/compare/rasn-derive-v0.15.2...rasn-derive-v0.15.3) - 2024-06-14

### Other
- *(ber)* don't allocate `2 + N` `BigInt`s when parsing OIDs ([#263](https://github.com/librasn/rasn/pull/263))

## [0.15.0](https://github.com/librasn/rasn/compare/rasn-derive-v0.14.0...rasn-derive-v0.15.0) - 2024-05-17

### Other
- Remove `backtraces` from `rasn`'s `default` feature ([#247](https://github.com/librasn/rasn/pull/247))

## [0.14.0](https://github.com/librasn/rasn/compare/rasn-derive-v0.13.1...rasn-derive-v0.14.0) - 2024-04-04

### Other
- Feat/identifier annotation ([#239](https://github.com/librasn/rasn/pull/239))

## [0.12.6](https://github.com/librasn/rasn/compare/rasn-derive-v0.12.5...rasn-derive-v0.12.6) - 2024-03-09

### Other
- *(macros)* Treat Unit Structs as ASN.1 NULL ([#227](https://github.com/librasn/rasn/pull/227))
- Fix calling the specified default fn
- Add default_initializer_fn optimisation

## [0.12.5](https://github.com/librasn/rasn/compare/rasn-derive-v0.12.4...rasn-derive-v0.12.5) - 2024-02-02

### Fixed
- *(macro)* recognize option references ([#219](https://github.com/librasn/rasn/pull/219))

## [0.12.1](https://github.com/XAMPPRocky/rasn/compare/rasn-derive-v0.12.0...rasn-derive-v0.12.1) - 2023-11-14

### Other
- Fix PER ObjectIdentifier, Alignment for Choice index encoding ([#202](https://github.com/XAMPPRocky/rasn/pull/202))

## [0.12.0](https://github.com/XAMPPRocky/rasn/compare/rasn-derive-v0.11.1...rasn-derive-v0.12.0) - 2023-11-12

### Fixed
- *(macros)* handle negative discriminants

### Other
- Add `Option<T::EXTENDED_VARIANTS>` for Choice, clippy cleanup for relevant macros ([#200](https://github.com/XAMPPRocky/rasn/pull/200))
- Feature/jer ([#187](https://github.com/XAMPPRocky/rasn/pull/187))
- Field_error improved, Boxed error `kind`, explicit naming also for `DecodeErrorKind` ([#197](https://github.com/XAMPPRocky/rasn/pull/197))
- run cargo fmt

## [0.11.0](https://github.com/XAMPPRocky/rasn/compare/rasn-derive-v0.10.6...rasn-derive-v0.11.0) - 2023-10-28

### Other
- Shared error module ([#164](https://github.com/XAMPPRocky/rasn/pull/164))

## [0.10.6](https://github.com/XAMPPRocky/rasn/compare/rasn-derive-v0.10.5...rasn-derive-v0.10.6) - 2023-10-26

### Other
- Add CI check for formatted files and reformat source ([#181](https://github.com/XAMPPRocky/rasn/pull/181))

## [0.10.4](https://github.com/XAMPPRocky/rasn/compare/rasn-derive-v0.10.3...rasn-derive-v0.10.4) - 2023-10-16

### Other
- four uper issues ([#177](https://github.com/XAMPPRocky/rasn/pull/177))

## [0.10.2](https://github.com/XAMPPRocky/rasn/compare/rasn-derive-v0.10.1...rasn-derive-v0.10.2) - 2023-10-10

### Other
- Fix/issue 165 ([#172](https://github.com/XAMPPRocky/rasn/pull/172))

## [0.10.0](https://github.com/XAMPPRocky/rasn/compare/rasn-derive-v0.9.5...rasn-derive-v0.10.0) - 2023-10-03

### Other
- Gensym field names ([#166](https://github.com/XAMPPRocky/rasn/pull/166))
- Delegate newtype EOC ([#163](https://github.com/XAMPPRocky/rasn/pull/163))
- Fix Result scoping ([#162](https://github.com/XAMPPRocky/rasn/pull/162))
- Fix/infinite recursion ([#157](https://github.com/XAMPPRocky/rasn/pull/157))
- Fix/constrained extension ([#156](https://github.com/XAMPPRocky/rasn/pull/156))

## [0.6.1](https://github.com/XAMPPRocky/rasn/compare/rasn-derive-v0.6.0...rasn-derive-v0.6.1) - 2023-07-11

### Other
- Add constraints to PKIX
- clippy
- Implement Unpacked Encoding Rules (UPER)
