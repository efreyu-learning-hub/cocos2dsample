# cocos2dsample


## How to build

#### Make sure you added -DCMAKE_OSX_ARCHITECTURES=x86_64 and -DDEBUG=1 to your cmake command line.
- -DCMAKE_OSX_ARCHITECTURES=x86_64 required to enable 64bit build even if you are using Apple Silicon.
- -DDEBUG=1 required to enable debug build that enables debug overlay.

```bash
cd cocos2dsample
cmake . -B build -DCMAKE_OSX_ARCHITECTURES=x86_64 -DDEBUG=1
```
