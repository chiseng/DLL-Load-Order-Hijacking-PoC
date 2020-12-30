# DLL-Search-Order-Hijacking-PoC

Small Proof-of-Concept on the search order hijacking method as referenced from https://attack.mitre.org/techniques/T1574/001/ on the explorer.exe binary that imports functions from the dwmapi.dll binary.

Platforms tested: Windows 7 SP1 x64 build.
Note: framework.h contains exports for the dwmapi.dll binary on windows 10 but PoC does not yet fully work.
