# mushclient-soundpack-launcher
An easy-to-use launcher for any type of MUSHclient-based soundpacks

This launcher was created since many people without great scripting knowledge wanted to create soundpacks easily, without the need  to program very much.
This project offers all the functions needed, including screen reader support and full audio functionalities.
I will update regularly to keep the current MUSHclient version updated.

# Getting Started

Any user who wants to create a soundpack for whatever mud needs to copy this project (or add it via git submodules) and create a world file inside the worlds folder which is called world.mcl. This file will be loaded on startup and all needed plugins will be injected automatically. Anything else (including additional plugin loading stuff) can be done inside this world file.

# Programming Advice

This launcher also offers all the advanced programming functionalities you'd expect. It bundles a LuaJIT with FFI included, which enables you to access external libraries if needed.

It also bundles ssl support as well as threading support, using the [llthreads library[(https://github.com/Neopallium/lua-llthreads).

The [penlight library](https://github.com/stevedonovan/Penlight) is included too, which extends the lua standard library with class-like tables and functionalities which enable pythonic programming, just in Lua.
