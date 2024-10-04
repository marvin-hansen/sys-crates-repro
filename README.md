# Repro 



Reproduces issue [2917 in rules_rust](https://github.com/bazelbuild/rules_rust/issues/2917)

Error:

```
cargo:rerun-if-env-changed=CC_SHELL_ESCAPED_FLAGS
CC_SHELL_ESCAPED_FLAGS = None
cargo:warning=liblz4/lib/lz4.c:224:11: fatal error: 'stdlib.h' file not found
cargo:warning=  224 | # include <stdlib.h>   /* malloc, calloc, free */
cargo:warning=      |           ^~~~~~~~~~
cargo:warning=1 error generated.

--stderr:
```