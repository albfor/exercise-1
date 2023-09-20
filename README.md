# Exercise 1

## Walkthrough
1. Create a directory called exercise-1 and move into it.

Install from source
-------------------

See the [Building Neovim](https://github.com/neovim/neovim/wiki/Building-Neovim) wiki page and [supported platforms](https://neovim.io/doc/user/support.html#supported-platforms) for details.

The build is CMake-based, but a Makefile is provided as a convenience.
After installing the dependencies, run the following command.

    make CMAKE_BUILD_TYPE=RelWithDebInfo
    sudo make install

To install to a non-default location:

    make CMAKE_BUILD_TYPE=RelWithDebInfo CMAKE_INSTALL_PREFIX=/full/path/
    make install

CMake hints for inspecting the build:

- `cmake --build build --target help` lists all build targets.
- `build/CMakeCache.txt` (or `cmake -LAH build/`) contains the resolved values of all CMake variables.
- `build/compile_commands.json` shows the full compiler invocations for each translation unit.
