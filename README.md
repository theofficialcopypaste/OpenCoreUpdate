# Hackintosh: OpenCore Update

## Requirement

* **A. Bootloader**

  Extensible Firmware Interface

  * [Acidanthera](https://github.com/acidanthera) / [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg)
    * Bootloader with development SDK.
      * [OpenCore Release](https://github.com/acidanthera/OpenCorePkg/releases)

* **B. Tools**
  
  Tools to update OpenCore EFI
  
  * [ic005k](https://github.com/ic005k) / [OCAuxiliaryTools](https://github.com/ic005k/OCAuxiliaryTools)
    * GUI-based Configurator for editing "config.plist" files for Acidanthera's OpenCore Boot Manager.
  * [rusty-bits](https://github.com/rusty-bits) / [octool](https://github.com/rusty-bits/octool) <sup>recommended</sup>
    * An OpenCore terminal based updater build from [Rust](https://www.rust-lang.org/).

* **C. Compare** <sup>optional</sup>

  An additional tool to compare config.plist with sample.plist.
  
  * [Araxis](https://www.araxis.com/) / [Araxis Merge](https://www.araxis.com/download/Merge2022.5809-macOS.dmg) 
    * Paid apps to compare different revisions of text files, program source code, XML and HTML files.
  * [corpnewt](https://github.com/corpnewt) / [OCConfigCompare](https://github.com/corpnewt/OCConfigCompare) 
    * Python script to compare two plists and list missing keys in either.
  * [meldmerge](https://meldmerge.org/) / [Homebrew](https://brew.sh/) / [meld](https://formulae.brew.sh/cask/meld)
    * Free apps to compare files, directories, and version controlled projects.


## Kexts

* **Nightly**
  * [Builds](https://dortania.github.io/builds/)

* **Release**
  * [Acidanthera](https://github.com/acidanthera)
    * [AirportBrcmFixup](https://github.com/acidanthera/AirportBrcmFixup) / [Release](https://github.com/acidanthera/AirportBrcmFixup/releases) 
    * [AppleALC](https://github.com/acidanthera/AppleALC) / [Release](https://github.com/acidanthera/AppleALC/releases)
                                                  



