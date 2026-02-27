# GitHub Copilot Instructions for Tarides Company Handbook

This repository is a template providing standard file boilerplate to encourage shared best practices for all projects created in the Tarides organization.

## Project Overview

This is a company handbook template repository that provides boilerplate files and guidelines for new projects at Tarides. It includes standard files like LICENSE.md, CONTRIBUTING.md, CODE_OF_CONDUCT.md, and project documentation templates.

## Coding Standards

### License and Copyright Headers

- This project is distributed under the MIT license.
- Every source file should start with a header comment specifying the license using an SPDX license identifier along with a copyright notice.
- For OCaml files, use the following format:

```ocaml
(* SPDX-License-Identifier: MIT
 * Copyright (c) <date> <author> <email>
 *)
```

### Copyright Holder Guidelines

- The holder on the copyright line is the name of individual contributors and/or their company.
- When adding significant new contributions to a file:
  - If there's already a copyright for your holder, it's not required to add the current year (but allowed). Never replace existing years.
  - If there's no line for your copyright holder, add one with the current year.

### OCaml Formatting

- This project uses OCaml version 5.2 and ocamlformat version 0.26.0.
- The `.ocamlformat` configuration specifies:
  - Profile: conventional
  - OCaml version: 5.2
  - Break infix: fit-or-vertical
  - Parse docstrings: true
- Always run ocamlformat on OCaml files before committing.

## Build System

- Uses Dune build system (check for `_build/` directory in `.gitignore`).
- Uses Opam for package management (check for `_opam/` directory in `.gitignore`).

## File Structure

- Keep standard boilerplate files at the root: README.md, LICENSE.md, CONTRIBUTING.md, CODE_OF_CONDUCT.md, CHANGES.md
- Build artifacts should be excluded via `.gitignore` (`_build/`, `_opam/`)
- Include Tarides.svg logo for branding

## Documentation

- README.md uses markdown with TODOs for template customization
- Sections should include: Synopsis, Installation, Documentation, Contribution
- Always reference Tarides branding at the bottom of README files

## General Guidelines

- When making changes, ensure they align with template-first approach
- Maintain consistency with existing file structure
- Keep boilerplate generic enough to work across different project types
- Document any new standard practices in the appropriate files
- Follow markdown best practices for documentation files
