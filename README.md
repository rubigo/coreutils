![rubigo-coreutils](coreutils.png)

Coreutils implemented in Rust, with a focus on usability, speed and security. 

## Utilities

name | version | status | coverage | docs
---: | :-----: | :----: | :------: | :---
[`yes`](https://github.com/rubigo/yes) | [![current tag](https://img.shields.io/github/tag/rubigo/yes.svg)](CHANGELOG.md) | [![travis build status](https://travis-ci.org/rubigo/yes.svg?branch=master)](https://travis-ci.org/rubigo/yes) | [![codecov](https://codecov.io/gh/rubigo/yes/branch/master/graph/badge.svg)](https://codecov.io/gh/rubigo/yes) | [![docs: published](https://img.shields.io/badge/docs-published-green.svg)](https://rubigo.github.io/coreutils/doc/rubigo_yes) 
[`true`](https://github.com/rubigo/true), [`false`](https://github.com/rubigo/true) | [![current tag](https://img.shields.io/github/tag/rubigo/true.svg)](CHANGELOG.md) | [![travis build status](https://travis-ci.org/rubigo/true.svg?branch=master)](https://travis-ci.org/rubigo/true) | [![codecov](https://codecov.io/gh/rubigo/true/branch/master/graph/badge.svg)](https://codecov.io/gh/rubigo/true) | [![docs: published](https://img.shields.io/badge/docs-published-green.svg)](https://rubigo.github.io/coreutils/doc/rubigo_true) 
[`pwd`](https://github.com/rubigo/pwd) | [![current tag](https://img.shields.io/github/tag/rubigo/pwd.svg)](CHANGELOG.md) | [![travis build status](https://travis-ci.org/rubigo/pwd.svg?branch=master)](https://travis-ci.org/rubigo/pwd) | [![codecov](https://codecov.io/gh/rubigo/pwd/branch/master/graph/badge.svg)](https://codecov.io/gh/rubigo/pwd) | [![docs: published](https://img.shields.io/badge/docs-published-green.svg)](https://rubigo.github.io/coreutils/doc/rubigo_pwd) 

## Specification

All utilities should more-or-less conform to the POSIX specification.
Additionally, they should be compatible with other implementations (GNU
coreutils, OpenBSD implementations).

Utilities should be kept as lean as possible, code should be reused as much as
possible. If available, security features on platforms should be used (like
`pledge` on BSD or `seccomp` on linux). 

Every feature and every part of the public API must have tests and be well
specified as well as documented.

If possible, implementations should be checked by line count (less is better),
efficiency (faster is better), syscall count (less are better) and improved.

## Philosophy

-   Do one thing and do it well.
-   One program gets one repository.
-   Shared functionality between programs should be outsourced into crates.
-   DRY — don't repeat yourself.
-   Keep everything well-documented.
-   If you can, keep the number of syscalls low.
-   Try to be as compatible as possible with existing implementations.
-   Have sane defaults, avoid over-customisability. 
-   Ease of use is most important.
