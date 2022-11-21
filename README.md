# OpenCoreUpdate

## Method 1:

### Using [rusty-bits](https://github.com/rusty-bits) octool

A small OpenCore project from [rusty-bits](https://github.com/rusty-bits) which directly update EFI from official branch [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg) repository. Why [octool](https://github.com/rusty-bits/octool)?

* Light
* Simple
* Easy to handle

#### Information

Help

```zsh
./octool -h
```
```zsh
SYNOPSIS
	./octool [options] [-o x.y.z] [config.plist]
OPTIONS
	-d  build debug version
	-h  print this help and exit
	-o x.y.z  select OpenCore version number
	-v  show octool version info
```

Editing

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

