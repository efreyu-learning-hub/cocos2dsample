# cocos2dsample

A sample cocos2d-x project demonstrating the **cocos2dx-debug** runtime node inspector.

This project is designed to help programmers and game developers study cocos2d-x and game programming concepts.

## About

This project showcases [cocos2dx-debug](Classes/cocos2d_debug/README.md) — an interactive ImGui-based debug inspector for cocos2d-x projects. The inspector allows you to:

- Browse and inspect the scene graph hierarchy in real-time
- View and modify node properties (position, scale, rotation, etc.)
- Debug complex scene transformations visually

The debug module is included as a git submodule in `Classes/cocos2d_debug/`.

## Requirements

- cocos2d-x (CMake-based project)
- C++17 or newer

## How to build

#### Make sure you added -DCMAKE_OSX_ARCHITECTURES=x86_64 and -DDEBUG=1 to your cmake command line.
- `-DCMAKE_OSX_ARCHITECTURES=x86_64` required to enable 64bit build even if you are using Apple Silicon.
- `-DDEBUG=1` required to enable debug build that enables debug overlay.

```bash
git clone --recursive <repo-url>
cd cocos2dsample
cmake . -B build -DCMAKE_OSX_ARCHITECTURES=x86_64 -DDEBUG=1
cmake --build build
```

If you already cloned without `--recursive`, initialize the submodule:
```bash
git submodule update --init --recursive
```

## Using the inspector in your own project

See the [cocos2dx-debug README](Classes/cocos2d_debug/README.md) for integration instructions.

## Contributing

Adjustments, ideas, and contributions are welcome. Feel free to open issues or submit pull requests.
