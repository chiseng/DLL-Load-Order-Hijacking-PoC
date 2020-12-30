# DLL-Search-Order-Hijacking-PoC

Small Proof-of-Concept on the search order hijacking method as referenced from https://attack.mitre.org/techniques/T1574/001/ on the explorer.exe binary that imports functions from dwmapi.dll.

### Error Codes

`Application could not be started 0xc0000005` which is thrown by ntdll.dll that a specific memory location cannot be accessed. Check for incorrect spelling of exports which results in a successful build but throws an exception when trying to export the function. 

### Notes

Platforms tested: Windows 7 SP1 x64 build.

`win7.h` contains exports for dwmapi.dll on windows 7 and `framework.h` contains exports for the  windows 10 but PoC does not yet fully work.

TODO:

Spawn shell from windows 10 target without crashing the system
