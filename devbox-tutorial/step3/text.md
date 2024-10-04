# Understand the devbox.json file

## Explain the dependecies
- Nix package manager (en vez de apt, explicar un poco)
- How locate new packates https://search.nixos.org/packages 
- Explain why devbox is required instad just nix packer manager
(abstracion de nix shells, lo hace en la carpeta local. Gestionar scrips, y se integracion con gh actions.)

See difference between python versions
Local



```bash
python --version
```{{exec}}
Devbox

```bash
devbox shell
python --version
```{{exec}}

Exit the shell with `exit`{{exec}}

(Init hook se corre siempre.) -> 


## Explain the scripts
- explain scripts in devbox.json
- the project in python shpould have a test (pytest) and a devbox script should run it
