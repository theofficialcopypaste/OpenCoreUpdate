# Hackintosh: OpenCore Update

### Apps / Tools

#### A. Extensible Firmware Interface (EFI)

| **Dev**                                       | **Download**                                                            | **Details**                     |
| --------------------------------------------- | ----------------------------------------------------------------------- | ------------------------------- |
| [Acidanthera](https://github.com/acidanthera) | [OpenCore Release](https://github.com/acidanthera/OpenCorePkg/releases) | Bootloader with development SDK |

#### B. Updater

| **Dev**                                     | **Download**                                                   | **Details**                                                                                   |
| ------------------------------------------- | -------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| [ic005k](https://github.com/ic005k)         | [OCAuxiliaryTools](https://github.com/ic005k/OCAuxiliaryTools) | GUI-based configurator for editing config.plist files for Acidanthera's OpenCore Boot Manager |
| [rusty-bits](https://github.com/rusty-bits) | [octool](https://github.com/rusty-bits/octool)                 | An OpenCore terminal based EFI updater build from [Rust](https://www.rust-lang.org/)          |

#### C. Plist editing

| **Dev**                                 | **Download**                                         | **Details**                                  |
| --------------------------------------- | ---------------------------------------------------- | -------------------------------------------- |
| [corpnewt](https://github.com/corpnewt) | [ProperTree](https://github.com/corpnewt/ProperTree) | Cross-platform GUI .plist editor             |
| [ic005k](https://github.com/ic005k)     | [Xplist](https://github.com/ic005k/Xplist)           | Lightweight .plist editor with rich features |

#### D. Compare (Optional).

| **Dev**                                 | **Download**                                                                | **Details**                                                                                       |
| --------------------------------------- | --------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| [Araxis](https://www.araxis.com/)       | [Araxis Merge](https://www.araxis.com/download/Merge2022.5809-macOS.dmg)    | Paid apps to compare different revisions of text files, program source code, .xml and .html files |
| [corpnewt](https://github.com/corpnewt) | [OCConfigCompare](https://github.com/corpnewt/OCConfigCompare)              | Python script to compare two .plists and list missing keys in either                              |
| [meldmerge](https://meldmerge.org/)     | [Homebrew](https://brew.sh/) and [meld](https://formulae.brew.sh/cask/meld) | Free apps to compare files, directories, and version controlled projects                          |

> **Note**: Personally, [octool](https://github.com/rusty-bits/octool) and [ProperTree](https://github.com/corpnewt/ProperTree) is enough to handle EFI update.

### Kexts

#### A. Dortania Builds

| **Dev**                                 | **Download**                                 | **Details**              |
| --------------------------------------- | -------------------------------------------- | ------------------------ |
| [Dortania](https://dortania.github.io/) | [Builds](https://dortania.github.io/builds/) | Recent debug and release |

#### B. Legacy

| **Dev**                                         | **Download**                                                  | **Details**              |
| ----------------------------------------------- | ------------------------------------------------------------- | ------------------------ |
| [khronokernel](https://github.com/khronokernel) | [Legacy Builds](https://github.com/khronokernel/Legacy-Kexts) | Legacy Kernel Extension  |

#### C. Alternative

| **Dev**                                                 | **Download**                                                                  | **Details**  |
| ------------------------------------------------------- | ----------------------------------------------------------------------------- | ------------ |
| [CloverHackyColor](https://github.com/CloverHackyColor) | [Release](https://github.com/CloverHackyColor/FakeSMC3_with_plugins/releases) | FakeSMC v3   |
