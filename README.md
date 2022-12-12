# Hackintosh: OpenCore Update

![OpenCore](https://img.shields.io/badge/Bootloader-OpenCore-purple)
![OS](https://img.shields.io/badge/OS-macOS-orange)
![Check](https://img.shields.io/badge/Status-Pass-brightgreen)
![GitHub issues](https://img.shields.io/github/issues/theofficialcopypaste/ASRockB460MSL-OC?color=blue&label=Issues)
![Information](https://img.shields.io/badge/Information-Tools-yellow)

**Table of Contents**

[Apps and Tools](https://github.com/theofficialcopypaste/OpenCoreUpdate#apps--tools) | [Kexts](https://github.com/theofficialcopypaste/OpenCoreUpdate#kexts) | [SSDT](https://github.com/theofficialcopypaste/OpenCoreUpdate/blob/main/README.md#ssdt) | [Recovery](https://github.com/theofficialcopypaste/OpenCoreUpdate#recovery)

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

![octool](https://user-images.githubusercontent.com/72515939/206939537-57a9147b-8a10-4c15-9f83-560da20ba144.png)

> **Note**: Using [octool](https://github.com/rusty-bits/octool) provide cleaner update. 

---

#### C. Plist editing

| **Dev**                                 | **Download**                                         | **Details**                                  |
| --------------------------------------- | ---------------------------------------------------- | -------------------------------------------- |
| [corpnewt](https://github.com/corpnewt) | [ProperTree](https://github.com/corpnewt/ProperTree) | Cross-platform GUI .plist editor             |
| [ic005k](https://github.com/ic005k)     | [Xplist](https://github.com/ic005k/Xplist)           | Lightweight .plist editor with rich features |


* **Propertree**

![PythonPropertree](https://user-images.githubusercontent.com/72515939/206940229-e8acaf52-f90f-41a9-bc28-1d1074f6e5e2.png)

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

#### B. Kext Updater

| **Dev**                                            | **Download**                                                            | **Details**       |
| -------------------------------------------------- | ----------------------------------------------------------------------- | ----------------- |
| [SL-Soft](https://www.sl-soft.de/en/kext-updater/) | [Release](https://update.kextupdater.de/kextupdater/Kext%20Updater.zip) | Kext Updater      |

* **KextUpdater**

![KextUpdater](https://user-images.githubusercontent.com/72515939/203808504-079c00b3-12fc-4809-9071-d5a7928d7916.png)

> **Note**: A small project on [Hackintosh-Forum.de](https://www.hackintosh-forum.de/) for pure version checking, the Kext Updater now offers an extensive range of functions that go beyond simply updating Kext´s.

---

#### C. Legacy

| **Dev**                                         | **Download**                                                  | **Details**              |
| ----------------------------------------------- | ------------------------------------------------------------- | ------------------------ |
| [khronokernel](https://github.com/khronokernel) | [Legacy Builds](https://github.com/khronokernel/Legacy-Kexts) | Legacy Kernel Extension  |

> **Note**: 32bit supported

---

#### D. Alternative

| **Dev**                                                 | **Download**                                                                  | **Details**  |
| ------------------------------------------------------- | ----------------------------------------------------------------------------- | ------------ |
| [CloverHackyColor](https://github.com/CloverHackyColor) | [Release](https://github.com/CloverHackyColor/FakeSMC3_with_plugins/releases) | FakeSMC3     |

> **Note**: An alternative SMC emulation kernel extension.

---

#### E. Slimmed Kext

| **Dev**                                         | **Download**                                                                         | **Details**                |
| ----------------------------------------------- | ------------------------------------------------------------------------------------ | -------------------------- |
| [dreamwhite](https://github.com/dreamwhite)     | [Release](https://github.com/dreamwhite/ChonkyAppleALC-Build/releases)               | Specific AppleHDA   |
| [dreamwhite](https://github.com/dreamwhite)     | [Release](https://github.com/dreamwhite/ChonkyIntelBluetoothFirmware-Build/releases) | Specific ITLWM |

* **AppleALC**

![Audio](https://user-images.githubusercontent.com/72515939/206940074-60454223-093e-4086-b968-7a8fa1bc7c74.png)

![Audio2](https://user-images.githubusercontent.com/72515939/206940081-bf2b6b45-75a9-4db4-b172-6c1f9d3e024c.png)

> **Note**: Dreamwhite's auto-generated list of AppleALC layout IDs available per each codec and auto-generated list of IntelBluetoothFirmware.kext available.

---

### SSDT

#### A. SSDTTime

| **Dev**                                 | **Download**                                                                 | **Details**        |
| --------------------------------------- | ---------------------------------------------------------------------------- | ------------------ |
| [corpnewt](https://github.com/corpnewt) | [Builds](https://github.com/corpnewt/SSDTTime/archive/refs/heads/master.zip) | SSDT/DSDT hotpatch |

* **SSDTTime**

![SSDTTime](https://user-images.githubusercontent.com/72515939/206939689-a5675d65-2a2c-4f52-9494-b61688af5b4b.png)

---

#### B. Guide

| **User**                                | **Link**                                                 | **Details**        |
| --------------------------------------- | -------------------------------------------------------- | ------------------ |
| [5T33Z0](https://github.com/5T33Z0)     | [Builds](https://github.com/5T33Z0/OC-Little-Translated) | SSDT/DSDT hotpatch |
| [CopyPaste](https://github.com/theofficialcopypaste) | [Samples](https://github.com/theofficialcopypaste/OpenCoreUpdate/tree/main/SSDT-Modular%20Sample) | SSDT Samples |

---

### Recovery

#### A.	gibMacRecovery (Latest)

| **Dev**                                 | **Download**                                                 | **Details**        		   |
| --------------------------------------- | ------------------------------------------------------------ | ------------------------------- |
| [corpnewt](https://github.com/corpnewt) | [gibMacRecovery](https://github.com/corpnewt/gibMacRecovery) | Linux, Mac, Windows (Standalone)|
| [corpnewt](https://github.com/corpnewt) | [gibMacOS](https://github.com/corpnewt/gibMacOS)             | Linux, Mac, Windows (under OpenCorePkg / Utilities / macrecovery |

* **gibMacRecovery**

![gibMacRecovery](https://user-images.githubusercontent.com/72515939/206939876-366ef688-c5c5-4348-a7f5-6e977ec6dbf1.png)

* **gibMacOS**

![gibMacOS](https://user-images.githubusercontent.com/72515939/206939805-df91a8df-e333-4ebe-bd8d-1c9345b138c7.png)
