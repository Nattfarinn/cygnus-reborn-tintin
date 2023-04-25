# Description
Cygnus: Reborn TinTin++ console UI configuration

![Example: Combat](https://github.com/Nattfarinn/cygnus-reborn/tintin/blob/main/examples/combat.png?raw=true)


# Installation
Download [latest](https://github.com/Nattfarinn/cygnus-reborn-tintin/releases/latest) release package and unpack it. As TinTin++ does not support relative paths it is necessary to rename directory to `cygnus-reborn-tintin` (without version suffix).

Create your own, character specific, configuration file (ie. `my_character.tin`) in the very same directory that contains `cygnus-reborn-tintin` directory with session connection:
```
#READ {cygnus-reborn-tintin/cygnus.tin};

#SESSION cygnus gra.cygnusreborn.pl 1111;
```

Optionally you can also store a character name and password just below the session to enable auto-logging:
```
#READ {cygnus-reborn-tintin/cygnus.tin};

#SESSION cygnus gra.cygnusreborn.pl 1111;
YourCharacterName;
YourPassword;
```

Run TinTin++ client with optional argument:
```
$ tt++ my_character.tin
```
