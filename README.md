# Nassembly
Learning nasm assembly

## Run Nassembly

For my system/setup only*

```sh
#!/bin/bash
nasm -f elf64 "${1}" -o "target/$(basename ${1%.*}).o"
ld -o "target/$(basename ${1%.*})" "target/$(basename ${1%.*}).o"
```
