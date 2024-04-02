# Unlocked map editor for the good old game Painkiller Black Edition v1.64
Do you like creating mods for good old games? Me too! One of my favorites is Painkiller Black Edition. Unfortunately, due to a bug, despite having an **original** Steam copy of the game, the map editor won't start up. Don't worry, in this repository you will find a bug fix that will allow you to create your own modifications!

## Ready to use executable
Just download the executable from this repo to: 

```path/to/steam/steamapps/common/Painkiller Black Edition/Bin/Editor```

## ModDB
The executable is also available on ModDB: [link](https://www.moddb.com/games/painkiller/downloads/paineditor-for-painkiller-black-edition-v164)

## DIY
Don't trust untrusted executables? Very good! Below is a step-by-step guide on how to fix the bug yourself.
1. Download the latest release of [Ghidra](https://github.com/NationalSecurityAgency/ghidra/releases)
2. Create a new project and import `pkedit.exe` from `path/to/steam/steamapps/common/Painkiller Black Edition/Bin/Editor`
3. Navigate to `004306c1`
4. Right click on the `JNZ` instruction -> Patch Instruction
5. Replace the `JNZ` instruction with `JN`
![image](https://github.com/LukaszBlasiak/pkedit/assets/14994840/302d3d87-be80-44d8-aa8d-c36debf5e45b)
6. File -> Export Program -> Format: `Original File` -> Ok
7. Happy modding :)
![image](https://github.com/LukaszBlasiak/pkedit/assets/14994840/a1dcf7cc-5391-4c8e-a25b-c0cd85156f8d)
