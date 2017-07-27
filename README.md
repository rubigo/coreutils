![rubigo-coreutils](img/coreutils.png)

Coreutils implemented in Rust, with a focus on usability, speed and security. 


## Goals

-   Do one thing and do it well.
-   One program gets one repository.
-   Shared functionality between programs can be split between multiple file.
-   Shared functionality between programs should be outsourced into crates.
-   DRY — don't repeat yourself.
-   Keep everything well-documented.
-   If you can, keep the number of syscalls low.
-   Try to be as compatible as possible with existing implementations.
-   Have sane defaults, avoid over-customisability. 
-   Ease of use is most important.

## Features

-   Cross-platform support (Linux, BSD, Windows).
-   Use local security features (`libseccomp`, BSD `pledge`) if available.
-   Small codebase, easy to audit.
