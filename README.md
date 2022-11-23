# Hackintosh: OpenCore Update

**Lists**

* [Apps and Tools](https://github.com/theofficialcopypaste/OpenCoreUpdate#apps--tools)
* [Kexts](https://github.com/theofficialcopypaste/OpenCoreUpdate#kexts)
* [SSDT](https://github.com/theofficialcopypaste/OpenCoreUpdate/blob/main/README.md#ssdt)

---

### Apps / Tools

#### A. Extensible Firmware Interface (EFI)

| **Dev**                                       | **Download**                                                            | **Details**                     |
| --------------------------------------------- | ----------------------------------------------------------------------- | ------------------------------- |
| [Acidanthera](https://github.com/acidanthera) | [OpenCore Release](https://github.com/acidanthera/OpenCorePkg/releases) | Bootloader with development SDK |
| [Acidanthera](https://github.com/acidanthera) | [OpenCore Binary Data](https://github.com/acidanthera/OcBinaryData)     | Binary Data |

* **OpenCore**

![OpenCore](https://user-images.githubusercontent.com/72515939/203320371-181058ca-3272-4ea0-a190-f11ef1ac0974.png)

---

#### B. Updater

| **Dev**                                     | **Download**                                                   | **Details**                                                                                   |
| ------------------------------------------- | -------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| [ic005k](https://github.com/ic005k)         | [OCAuxiliaryTools](https://github.com/ic005k/OCAuxiliaryTools) | GUI-based configurator for editing config.plist files for Acidanthera's OpenCore Boot Manager |
| [rusty-bits](https://github.com/rusty-bits) | [octool](https://github.com/rusty-bits/octool)                 | An OpenCore terminal based EFI updater build from [Rust](https://www.rust-lang.org/)          |

* **OCAuxiliary**

![ACAT](https://user-images.githubusercontent.com/72515939/203323165-e1e06101-d545-4f19-b0c5-9c68a6db85f7.png)

* **octool**

```zsh
SYNOPSIS
	./octool [options] [-o x.y.z] [config.plist]
OPTIONS
	-d  build debug version
	-h  print this help and exit
	-o x.y.z  select OpenCore version number
	-v  show octool version info
```
```zsh
Navigation: arrow keys or some standard vi keys
          'up'/'k'            jump to top of section
              ^                       't'
              |                        ^
'left'/'h' <-- --> 'right'/'l'         |
              |                        v
              v                       'b'
          'down'/'j'          jump to bottom of section
```

> **Note**: Using [octool](https://github.com/rusty-bits/octool) provide cleaner update. 

---

#### C. Plist editing

| **Dev**                                 | **Download**                                         | **Details**                                  |
| --------------------------------------- | ---------------------------------------------------- | -------------------------------------------- |
| [corpnewt](https://github.com/corpnewt) | [ProperTree](https://github.com/corpnewt/ProperTree) | Cross-platform GUI .plist editor             |
| [ic005k](https://github.com/ic005k)     | [Xplist](https://github.com/ic005k/Xplist)           | Lightweight .plist editor with rich features |


* **Propertree**

![Propertree](https://user-images.githubusercontent.com/72515939/203320853-96e6113c-83c0-4a61-95fb-39cad68a2f4e.png)

> **Note**: macOS Monterey and above, [ProperTree](https://github.com/corpnewt/ProperTree) require `python-tk@3.10` via [Homebrew](https://brew.sh/). 

```zsh
brew install python-tk@3.10 
```

---

#### D. Compare (Optional).

| **Dev**                                 | **Download**                                                                | **Details**                                                                                       |
| --------------------------------------- | --------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| [Araxis](https://www.araxis.com/)       | [Araxis Merge](https://www.araxis.com/download/Merge2022.5809-macOS.dmg)    | Paid apps to compare different revisions of text files, program source code, .xml and .html files |
| [corpnewt](https://github.com/corpnewt) | [OCConfigCompare](https://github.com/corpnewt/OCConfigCompare)              | Python script to compare two .plists and list missing keys in either                              |
| [meldmerge](https://meldmerge.org/)     | [Homebrew](https://brew.sh/) and [meld](https://formulae.brew.sh/cask/meld) | Free apps to compare files, directories, and version controlled projects                          |

* **Araxis Merge**

![Araxis](https://user-images.githubusercontent.com/72515939/203319617-9db8e6f6-95a1-4266-b910-78fbb398b4bc.png)

---

### Kexts

#### A. Dortania Builds

| **Dev**                                 | **Download**                                 | **Details**              |
| --------------------------------------- | -------------------------------------------- | ------------------------ |
| [Dortania](https://dortania.github.io/) | [Builds](https://dortania.github.io/builds/) | Recent debug and release |

* **Builds**

![Builds](https://user-images.githubusercontent.com/72515939/203321357-3e44bd4a-56fe-4225-b386-f4212f6a7838.png)

> **Note**: Most recent and updated version. 

---

#### B. Legacy

| **Dev**                                         | **Download**                                                  | **Details**              |
| ----------------------------------------------- | ------------------------------------------------------------- | ------------------------ |
| [khronokernel](https://github.com/khronokernel) | [Legacy Builds](https://github.com/khronokernel/Legacy-Kexts) | Legacy Kernel Extension  |

* **Legacy Builds**

![Legacy](https://user-images.githubusercontent.com/72515939/203321674-e7b5c057-b607-430d-8b94-0aa56991e058.png)

> **Note**: 32bit supported

---

#### C. Alternative

| **Dev**                                                 | **Download**                                                                  | **Details**  |
| ------------------------------------------------------- | ----------------------------------------------------------------------------- | ------------ |
| [CloverHackyColor](https://github.com/CloverHackyColor) | [Release](https://github.com/CloverHackyColor/FakeSMC3_with_plugins/releases) | FakeSMC3     |

* **FakeSMC3**

![FakeSMC3](https://user-images.githubusercontent.com/72515939/203321934-3a9465e0-a598-48c0-a343-de72412b5564.png)

> **Note**: An alternative SMC emulation kernel extension.

#### D. Slimmed Kext

| **Dev**                                         | **Download**                                                                         | **Details**                |
| ----------------------------------------------- | ------------------------------------------------------------------------------------ | -------------------------- |
| [dreamwhite](https://github.com/dreamwhite)     | [Release](https://github.com/dreamwhite/ChonkyAppleALC-Build/releases)               | Specific AppleHDA   |
| [dreamwhite](https://github.com/dreamwhite)     | [Release](https://github.com/dreamwhite/ChonkyIntelBluetoothFirmware-Build/releases) | Specific ITLWM |

![AppleALC](https://user-images.githubusercontent.com/72515939/203340882-5748e0db-1233-49b8-b45f-923c4a4e72b5.png)

> **Note**: Dreamwhite's auto-generated list of AppleALC layout IDs available per each codec and auto-generated list of IntelBluetoothFirmware.kext available.


### SSDT

#### A. SSDTTime

| **Dev**                                 | **Download**                                                                 | **Details**        |
| --------------------------------------- | ---------------------------------------------------------------------------- | ------------------ |
| [corpnewt](https://github.com/corpnewt) | [Builds](https://github.com/corpnewt/SSDTTime/archive/refs/heads/master.zip) | SSDT/DSDT hotpatch |

#### B. Guide

| **User**                                | **Link**                                                 | **Details**        |
| --------------------------------------- | -------------------------------------------------------- | ------------------ |
| [5T33Z0](https://github.com/5T33Z0)     | [Builds](https://github.com/5T33Z0/OC-Little-Translated) | SSDT/DSDT hotpatch |
