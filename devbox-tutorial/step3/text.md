# Understand the devbox.json file

## Explain the dependecies
- Nix package manager
- How locate new packates https://search.nixos.org/packages
- Explain why devbox is required instad just nix packer manager

See difference between python versions
Local

```bash
python --version
``` {{exec}}
Devbox

```bash
devbox shell
python --version
```{{exec}}

Exit the shell with `exit`{{exec}}

## Explain the scripts
- explain scripts in devbox.json
- the project in python shpould have a test (pytest) and a devbox script should run it
