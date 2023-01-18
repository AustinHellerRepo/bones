# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## Unreleased

### Chore

 - <csr-id-27252465ad0506ff2f8c377531fa079ec64d1750/> add missing crate descriptions.

### Documentation

 - <csr-id-a69389412d22b8cb48bab0ed96d739b0fee35348/> document source repository in cargo manifest.
   The `repository` key under `bones_ecs` previously pointed to https://github.com/fishfolk/jumpy.
   
   This updates this to point to the bones repo, and also adds the `repository` key to the other
   crates in the repository.

### New Features

 - <csr-id-6de087822484f866d606ea1935b9cae34e33aa2f/> add `TypeUlidDynamic` trait.
   `TypeUlidDynamic` is useful for creating trait objects such as `Box<dyn TypeUlidDynamic>`
   which isn't possible with the `TypeUlid` trait directly.

### New Features (BREAKING)

 - <csr-id-59f5e67d42de57a33dd302443a8a04427126a5be/> have `TypeUlid` trait require an associated constant instead of a function.
   This makes it possible to access the type's Ulid at compile time,
   possibly in const functions.
 - <csr-id-d74cec66c8e4db5f8d287f4e619d172d0f9c8b91/> use `TypeUlid`s instead of `TypeUuid`s.
   Creates a new type_ulid crate and uses it's `TypeUlid` trait instead of
   `TypeUuid` in bones_ecs.

### Commit Statistics

<csr-read-only-do-not-edit/>

 - 5 commits contributed to the release over the course of 20 calendar days.
 - 5 commits were understood as [conventional](https://www.conventionalcommits.org).
 - 5 unique issues were worked on: [#13](https://github.com/fishfolk/bones/issues/13), [#27](https://github.com/fishfolk/bones/issues/27), [#28](https://github.com/fishfolk/bones/issues/28), [#37](https://github.com/fishfolk/bones/issues/37), [#65](https://github.com/fishfolk/bones/issues/65)

### Commit Details

<csr-read-only-do-not-edit/>

<details><summary>view details</summary>

 * **[#13](https://github.com/fishfolk/bones/issues/13)**
    - use `TypeUlid`s instead of `TypeUuid`s. ([`d74cec6`](https://github.com/fishfolk/bones/commit/d74cec66c8e4db5f8d287f4e619d172d0f9c8b91))
 * **[#27](https://github.com/fishfolk/bones/issues/27)**
    - add `TypeUlidDynamic` trait. ([`6de0878`](https://github.com/fishfolk/bones/commit/6de087822484f866d606ea1935b9cae34e33aa2f))
 * **[#28](https://github.com/fishfolk/bones/issues/28)**
    - have `TypeUlid` trait require an associated constant instead of a function. ([`59f5e67`](https://github.com/fishfolk/bones/commit/59f5e67d42de57a33dd302443a8a04427126a5be))
 * **[#37](https://github.com/fishfolk/bones/issues/37)**
    - document source repository in cargo manifest. ([`a693894`](https://github.com/fishfolk/bones/commit/a69389412d22b8cb48bab0ed96d739b0fee35348))
 * **[#65](https://github.com/fishfolk/bones/issues/65)**
    - add missing crate descriptions. ([`2725246`](https://github.com/fishfolk/bones/commit/27252465ad0506ff2f8c377531fa079ec64d1750))
</details>
