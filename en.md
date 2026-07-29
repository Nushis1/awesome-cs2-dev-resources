# awesome-cs2-dev-resources

🇵🇱 [Polski](pl.md) | 🇬🇧 [English](en.md)

A curated list of GitHub repositories and C++ libraries useful for working with the Source 2 engine / Counter-Strike 2 - SDKs, offset generators, memory analysis tools, server and plugin frameworks, demo parsers, and libraries for graphics, audio, and image processing.

> This repository is for informational/educational purposes only - a collection of publicly available open-source projects and official Valve documentation and graphics/audio libraries.

## Table of contents

- [SDKs and base frameworks](#sdks-and-base-frameworks)
- [Memory analysis and offset generation](#memory-analysis-and-offset-generation)
- [Reverse engineering and research frameworks](#reverse-engineering-and-research-frameworks)
- [External tools and open-source projects](#external-tools-and-open-source-projects)
- [Server and plugin development](#server-and-plugin-development)
- [Demo and replay tools](#demo-and-replay-tools)
- [Utility tools](#utility-tools)
- [Official Valve resources](#official-valve-resources)
- [Top picks](#top-picks)
- [C++ effects libraries](#c-effects-libraries)
  - [Rendering and graphics](#rendering-and-graphics)
  - [Particle systems](#particle-systems)
  - [Shader systems](#shader-systems)
  - [Audio effects](#audio-effects)
  - [Image processing](#image-processing)
  - [Libraries especially useful for CS2 tooling](#libraries-especially-useful-for-cs2-tooling)

---

## SDKs and base frameworks

| Repository | Link | Description |
| --- | --- | --- |
| **bruhmoment21/cs2-sdk** | https://github.com/bruhmoment21/cs2-sdk | SDK/base for Counter-Strike 2 written in C++. Supports DirectX 11 and Vulkan, Windows and Linux. Includes function hooking (funchook), a disassembler (distorm), a GUI interface (ImGui), and a signature system (STB). MIT license. Around 418 stars. |
| **uraioa/cs2sdk** | https://github.com/uraioa/cs2sdk | Fork of the cs2-sdk project (v1 branch). C++ SDK base with ESP, rendering, and RCS (Recoil Control System) support. |
| **neverlosecc/source2gen** | https://github.com/neverlosecc/source2gen | Automatic SDK generator for games built on the Source 2 engine (CS2, Dota 2, Half-Life: Alyx, etc.). Cross-platform, generates headers compatible with C++23, C23, and IDA. |
| **neverlosecc/source2sdk** | https://github.com/ccsimplyspolit/CS2-SDK-Reference/tree/main/source2sdk | Generated Source 2 SDK for various games. Each game has its own branch (CS2, Dota, etc.). |

## Memory analysis and offset generation

| Repository | Link | Description |
| --- | --- | --- |
| **a2x/cs2-dumper** | https://github.com/a2x/cs2-dumper | The most popular tool for generating offsets and interfaces for CS2 (~2181 stars, 334 forks). Written in Rust using memflow. Supports Windows and Linux. Generates code for C#, C++, Rust, and JSON. |
| **scros22/cs2-universal-offsets** | https://github.com/scros22/cs2-universal-offsets | External SDK generator for CS2 written in Rust. Reads a running cs2.exe process and generates a C++ header file structure containing schemas, signatures, offsets, interfaces, vtables, and button definitions. Around 70 stars. |
| **sezzyaep/CS2-OFFSETS** | https://github.com/sezzyaep/CS2-OFFSETS | Ready-made, static offsets and interfaces for CS2 in multiple languages (C#, C++, Python, Rust, JSON, YAML). No dumper needed - just download the current files. Around 194 stars. |
| **a2x/cs2-analyzer** | https://github.com/a2x/cs2-analyzer | An actively developed offline version of the cs2-dumper project, also available as a web demo. |
| **dr-NHA/CS2-Schema-System-Dumper-CE** | https://github.com/dr-NHA/CS2-Schema-System-Dumper-CE | A CS2 system schema dumping tool based on Cheat Engine. |

## Reverse engineering and research frameworks

| Repository | Link | Description |
| --- | --- | --- |
| **Amiralisa5/Counter-Strike-2-Reverse-Engineering-Framework** | https://github.com/Amiralisa5/Counter-Strike-2-Reverse-Engineering-Framework | Aspasia - a C++ research framework for reverse engineering and prototyping mechanics in CS2. Created as a master's thesis at UC3M. Includes modules for entity and movement analysis, plus example implementations. |
| **Travers9483/mcp-cheat-engine** | https://github.com/Travers9483/mcp-cheat-engine | An MCP server that lets AI assistants control Cheat Engine, x64dbg, and Ghidra. Supports memory scanning, reading, writing, disassembly, and other operations through a shared interface. |

## External tools and open-source projects

| Repository | Link | Description |
| --- | --- | --- |
| **RvD-Projects/External-CheatEngine** | https://github.com/RvD-Projects/External-CheatEngine | A modern C++ project with modular architecture, automatic offset updates, and build pipelines. |
| **danielkrupinski/Osiris** | https://github.com/danielkrupinski/Osiris | A cross-platform project with a Panorama UI-based interface. |
| **ByteCorum/DragonBurn** | https://github.com/ByteCorum/DragonBurn | An external, kernel-mode project that uses memory reading only. |
| **IMXNOOBX/cs2-external-esp** | https://github.com/IMXNOOBX/cs2-external-esp | A simple project with a Discord/GDI overlay, designed with clarity and performance in mind. |
| **Valthrun/valthrun-cs2** | https://github.com/Valthrun/valthrun-cs2 | A project using only kernel-mode memory reading. |
| **avitran0/deadlocked** | https://github.com/avitran0/deadlocked | A Linux-only project. |

## Server and plugin development

| Repository | Link | Description |
| --- | --- | --- |
| **roflmuffin/CounterStrikeSharp** | https://github.com/roflmuffin/CounterStrikeSharp | A framework for writing server-side plugins for Counter-Strike 2 in C#. |
| **antonpup/CounterStrike2GSI** | https://github.com/antonpup/CounterStrike2GSI | A C# library for communicating with CS2's Game State Integration (GSI) system. |
| **shobhit-pathak/MatchZy** | https://github.com/shobhit-pathak/MatchZy | A plugin for organizing practice sessions, pugs, scrims, and matches, with Get5 support. |
| **B3none/cs2-retakes** | https://github.com/B3none/cs2-retakes | An implementation of the Retakes mode for CS2, based on an earlier version made for CS:GO. |

## Demo and replay tools

| Repository | Link | Description |
| --- | --- | --- |
| **markus-wa/demoinfocs-golang** | https://github.com/markus-wa/demoinfocs-golang | A Counter-Strike 2 demo parser written in Go. |
| **LaihoE/demoparser** | https://github.com/LaihoE/demoparser | A CS2 replay parser available for Python and JavaScript. |

## Utility tools

| Repository | Link | Description |
| --- | --- | --- |
| **FN-FAL113/cs2-server-picker** | https://github.com/FN-FAL113/cs2-server-picker | A lightweight, portable server picker for CS2 and Deadlock. |
| **Jyben/cs2-mm-server-picker** | https://github.com/Jyben/cs2-mm-server-picker | A matchmaking server picker for Windows and Linux. |
| **JohnTimmermann/JTs-Hud** | https://github.com/JohnTimmermann/JTs-Hud | A HUD manager using GSI and a Node.js server with WebSockets. |
| **drweissbrot/cs-hud** | https://github.com/drweissbrot/cs-hud | A custom spectator HUD for Counter-Strike. |
| **Flowtter/crispy** | https://github.com/Flowtter/crispy | An ML platform for automatically creating game montages using neural networks that detect the most exciting moments. |
| **joedwards32/CS2** | https://github.com/joedwards32/CS2 | A Docker image for a dedicated CS2 server. |
| **armync/ArminC-AutoExec** | https://github.com/armync/ArminC-AutoExec | A thoroughly documented and analyzed autoexec file for CS2, free of misconfigurations. |

## Official Valve resources

| Resource | Link | Description |
| --- | --- | --- |
| **CS2 Workshop Tools** | https://developer.valvesoftware.com/wiki/Counter-Strike_2_Workshop_Tools | Official Valve documentation on creating mods for CS2: level design, scripting, models, materials, particle effects, Source Filmmaker, and the scripting API. |
| **Source SDK 2013** | https://github.com/ValveSoftware/source-sdk-2013 | Valve's official repository containing the Source SDK 2013 for the Source 1 engine. |
| **Source-1-Games** | https://github.com/ValveSoftware/Source-1-Games | Official repositories for games built on the Source 1 engine. |

## Top picks

| Category | Recommended project | Why |
| --- | --- | --- |
| Offsets and memory analysis | **a2x/cs2-dumper** | The most actively developed and widely used offset/interface dumper for CS2 (~2.1k stars). |
| SDK generator | **scros22/cs2-universal-offsets** | Automatically generates complete SDK headers without manual analysis. |
| Base SDK / framework | **bruhmoment21/cs2-sdk** | The most popular open-source base for CS2-related projects. |
| Source 2 SDK generator | **neverlosecc/source2gen** | A universal tool for generating SDK headers for many Source 2-based games. |

---

## C++ effects libraries

General-purpose C++ libraries for graphics, audio, and image processing - useful across many projects, not necessarily tied to CS2.

### Rendering and graphics

| Library | Link | Description |
| --- | --- | --- |
| **OpenGL** | https://www.khronos.org/opengl/ | Cross-platform API for 2D/3D graphics rendering. The de facto standard for GPU-accelerated graphics. |
| **DirectX 11/12** | https://learn.microsoft.com/en-us/windows/win32/directx | Microsoft's graphics API for Windows. DirectX 11 is widely used in games, while DirectX 12 provides low-level GPU control. |
| **Vulkan** | https://www.khronos.org/vulkan/ | A modern, cross-platform, low-overhead graphics API with direct GPU control. |
| **SDL2** | https://www.libsdl.org/ | A cross-platform library for windowing, user input, and graphics via OpenGL and Direct3D. |
| **SFML** | https://www.sfml-dev.org/ | An object-oriented C++ library built on OpenGL for graphics, windowing, audio, and networking. |
| **GLFW** | https://www.glfw.org/ | A lightweight library for creating windows with an OpenGL context and handling keyboard, mouse, and controllers. |
| **Dear ImGui** | https://github.com/ocornut/imgui | An immediate-mode GUI library for C++. Supports OpenGL, DirectX, and Vulkan. |
| **bgfx** | https://github.com/bkaradzic/bgfx | A cross-platform rendering library unifying OpenGL, DirectX, Vulkan, and Metal. |
| **Magnum** | https://magnum.graphics/ | A lightweight, modular C++11 graphics engine for 2D and 3D applications. |
| **Ogre3D** | https://ogre3d.org/ | A scene-based 3D graphics engine with a flexible plugin architecture. |

### Particle systems

| Library | Link | Description |
| --- | --- | --- |
| **ParticleUniverse** | https://github.com/ParticleUniverse/ParticleUniverse | An open-source particle system engine for Ogre3D - usable for effects like fire, smoke, and explosions. |

### Shader systems

| Library / Tool | Link | Description |
| --- | --- | --- |
| **GLSL** | https://www.khronos.org/opengl/wiki/OpenGL_Shading_Language | A high-level shading language for OpenGL. |
| **HLSL** | https://learn.microsoft.com/en-us/windows/win32/direct3dhlsl/dx-graphics-hlsl | Microsoft's shading language for DirectX. |
| **SPIR-V** | https://www.khronos.org/spirv/ | An intermediate shader format used by Vulkan and OpenGL. |
| **ShaderConductor** | https://github.com/microsoft/ShaderConductor | A Microsoft tool for compiling shaders across APIs (HLSL → GLSL/SPIR-V/MSL). |
| **OptiX** | https://developer.nvidia.com/optix | NVIDIA's ray-tracing engine with a C++ API for real-time ray-tracing effects. |

### Audio effects

| Library | Link | Description |
| --- | --- | --- |
| **OpenAL** | https://www.khronos.org/openal/ | A cross-platform 3D audio API. The standard for spatial audio in games. |
| **OpenAL Soft** | https://openal-soft.org/ | An open-source OpenAL implementation with HRTF support. Can replace the original library without code changes. |
| **miniaudio** | https://github.com/mackron/miniaudio | A very lightweight, single-file C library for audio playback and recording. |
| **SDL_mixer** | https://www.libsdl.org/projects/SDL_mixer/ | An audio mixing library built on SDL2. Supports WAV, MP3, OGG, and many other formats. |
| **FMOD** | https://www.fmod.com/ | A professional game audio engine with a C++ API and sound-design tools. Free for indie projects. |
| **Wwise** | https://www.audiokinetic.com/products/wise/ | Professional audio middleware used in AAA productions. Provides a C++ API. |
| **RtAudio** | https://www.music.mcgill.ca/~gary/rtaudio/ | A C++ library for real-time audio input and output. Supports ALSA, CoreAudio, and WASAPI. |
| **JUCE** | https://juce.com/ | A C++ framework for building audio applications and VST, AU, and AAX plugins. |
| **SoundTouch** | https://www.surina.net/soundtouch/ | A library for changing playback tempo and pitch without quality loss. |
| **libsndfile** | https://libsndfile.github.io/libsndfile/ | A library for reading and writing audio files (WAV, AIFF, FLAC, and others). |
| **PortAudio** | http://www.portaudio.com/ | A cross-platform C library for audio input and output. |

### Image processing

| Library | Link | Description |
| --- | --- | --- |
| **OpenCV** | https://opencv.org/ | The most popular C++ library for image processing and computer vision. Includes over 2500 algorithms. |
| **stb_image** | https://github.com/nothings/stb | A single-file library for loading images (PNG, JPEG, BMP, TGA, etc.). |
| **stb_image_write** | https://github.com/nothings/stb | A single-file library for writing images (PNG, JPEG, BMP). |
| **FreeImage** | http://freeimage.sourceforge.net/ | An open-source library for reading and writing many image formats. |
| **libpng** | http://www.libpng.org/pub/png/libpng.html | A library for handling PNG files. |
| **libjpeg** | http://www.ijg.org/ | A library for reading and writing JPEG files. |
| **OpenEXR** | https://openexr.com/ | A library for handling HDR images in the OpenEXR format. |
| **Magick++** | https://imagemagick.org/script/index.php | A C++ interface for ImageMagick, supporting over 200 image formats. |
| **CImg** | http://cimg.eu/ | A lightweight C++ template library for image processing. |
| **Boost.GIL** | https://www.boost.org/doc/libs/release/libs/gil/ | An image-processing framework that is part of the Boost library. |
| **Halide** | https://halide-lang.org/ | A language and compiler designed for efficient image processing and AI applications. |
| **Intel IPP** | https://www.intel.com/content/www/us/en/developer/tools/oneapi/ipp.html | An optimized C/C++ library for image and signal processing on Intel processors. |

### Libraries especially useful for CS2 tooling

Context: projects using Present hooking, overlays, memory analysis, or a custom interface.

| Library | Link | Use case |
| --- | --- | --- |
| **Dear ImGui** | https://github.com/ocornut/imgui | Building menus and overlay interfaces. Used in cs2-sdk and many other open-source projects. |
| **funchook** | https://github.com/kubo/funchook | A function-hooking library (e.g., hooking Present in DirectX 11 or Vulkan). |
| **distorm** | https://github.com/gdabah/distorm | An x86/x64 disassembler used for code analysis and signature scanning. |
| **memflow** | https://github.com/memflow/memflow | A cross-platform memory-reading framework used by, among others, cs2-dumper. |
| **OpenCV** | https://opencv.org/ | Image processing, color conversion, contour detection, and image analysis. |
| **stb_image** | https://github.com/nothings/stb | Loading textures for user interfaces and other graphical elements. |
| **OpenGL** | https://www.khronos.org/opengl/ | A popular rendering API used for building graphical applications and overlays. |
| **Vulkan** | https://www.khronos.org/vulkan/ | A modern graphics API useful for projects using Vulkan as the rendering backend. |
| **SDL2** | https://www.libsdl.org/ | Window handling, user input, and the basics of cross-platform applications. |
| **miniaudio** | https://github.com/mackron/miniaudio | A lightweight audio library for custom tools and C++ applications. |

---

## License / Note

This document is only a collection of links to publicly available repositories and libraries. Each project has its own license - check it before use. Links to "external cheat" / offset dumper tools are listed here for informational purposes (reverse engineering, research on the Source 2 engine); using them in an online game may violate Valve's/VAC's terms of service.
