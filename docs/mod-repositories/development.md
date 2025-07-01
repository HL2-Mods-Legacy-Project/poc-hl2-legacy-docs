# Development

## Requirements

Everything below with the same version or higher:

- [poc-hl2-legacy-installer/built with](https://github.com/HL2-Mods-Legacy-Project/poc-hl2-legacy-installer/blob/v1.x/README.md#built-with)

## Cloning the repository

```text
git clone --recurse-submodules https://github.com/HL2-Mods-Legacy-Project/<mod repository>.git
```

## Building the installer

Open PowerShell and do the following:

```powershell
cd scripts
.\build_all.ps1
```

## Submodules

### Update all submodules

```text
git submodule update --remote --recursive
git add .
git commit -m "Update submodules"
git push
```

### Mod Installer

#### Update

```text
git submodule update --remote --recursive gitmodules/mod-installer
git add .
git commit -m "Update submodule mod-installer"
git push
```

#### Change the branch

```text
git submodule update --remote --recursive gitmodules/mod-installer
git submodule set-branch -b <branch> gitmodules/mod-installer
git submodule update --remote --recursive gitmodules/mod-installer
git add .
git commit -m "Change submodule gitmodules/mod-installer branch."
git push
```

### Utilities

#### Update

```text
git submodule update --remote --recursive gitmodules/utilities
git add .
git commit -m "Update submodule utilities"
git push
```
