# cppstarter

Starter C++ repo using CMake, vcpkg (manifest mode), and VS Code.

## Prereqs

- CMake 3.24+
- Ninja
- vcpkg (set `VCPKG_ROOT`)
- VS Code + CMake Tools extension

## Build

From VS Code:

1. Open the folder.
2. CMake Tools picks the `vcpkg` preset.
3. Build or Debug.

From terminal:

```powershell
cmake --preset vcpkg
cmake --build --preset vcpkg
```
