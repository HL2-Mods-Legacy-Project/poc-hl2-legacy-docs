# Development

## Requirements

Everything below with the same version or higher:

- [poc-hl2-legacy-installer/built with](https://github.com/HL2-Mods-Legacy-Project/poc-hl2-legacy-installer/blob/v1.x/README.md#built-with)
- [poc-hl2-legacy-utilities/built with](https://github.com/HL2-Mods-Legacy-Project/poc-hl2-legacy-utilities/blob/master/README.md#built-with)

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

Open PowerShell and do the following:

```powershell
gitmodules\utilities\submodule-update.ps1 gitmodules\mod-installer
```

#### Change the branch

Open PowerShell and do the following:

```powershell
gitmodules\utilities\submodule-set-branch.ps1 gitmodules\mod-installer <branch>
```

### Utilities

#### Update

Open PowerShell and do the following:

```powershell
gitmodules\utilities\submodule-update.ps1 gitmodules\utilities
```
