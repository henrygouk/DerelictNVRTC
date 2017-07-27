DerelictNVRTC
=============

Dynamic bindings to NVRTC for the D programming language.

Usage
-----

Similar to other Derelict-based dynamic bindings, simply call `DerelictNVRTC.load()` and begin using NVRTC!

```
    import std.stdio : writeln;
    import derelict.nvrtc;

    void main(string[] args)
    {
        DerelictNVRTC.load();

        int major, minor;

        nvrtcVersion(&major, &minor);
        writeln("NVRTC version ", major, ".", minor);
    }
```