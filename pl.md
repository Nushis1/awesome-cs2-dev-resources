# awesome-cs2-dev-resources

Zbiór linków i notatek na temat repozytoriów GitHub oraz bibliotek C++ przydatnych przy pracy z silnikiem Source 2 / Counter-Strike 2 — SDK, generatory offsetów, narzędzia do analizy pamięci, frameworki do serwerów i pluginów, parsery dem, a także biblioteki do grafiki, dźwięku i przetwarzania obrazu.

> Repozytorium ma charakter wyłącznie informacyjny/edukacyjny — zestawienie publicznie dostępnych projektów open source oraz oficjalnej dokumentacji Valve i bibliotek graficznych/audio.

## Spis treści

- [SDK i bazowe frameworki](#sdk-i-bazowe-frameworki)
- [Analiza pamięci i generowanie offsetów](#analiza-pamięci-i-generowanie-offsetów)
- [Reverse engineering i frameworki badawcze](#reverse-engineering-i-frameworki-badawcze)
- [Narzędzia zewnętrzne i projekty open source](#narzędzia-zewnętrzne-i-projekty-open-source)
- [Tworzenie serwerów i pluginów](#tworzenie-serwerów-i-pluginów)
- [Narzędzia do dem i powtórek](#narzędzia-do-dem-i-powtórek)
- [Narzędzia pomocnicze](#narzędzia-pomocnicze)
- [Oficjalne zasoby Valve](#oficjalne-zasoby-valve)
- [Najważniejsze projekty](#najważniejsze-projekty)
- [Biblioteki C++ do efektów](#biblioteki-c-do-efektów)
  - [Renderowanie i grafika](#renderowanie-i-grafika)
  - [Systemy cząsteczek](#systemy-cząsteczek)
  - [Systemy shaderów](#systemy-shaderów)
  - [Efekty dźwiękowe](#efekty-dźwiękowe)
  - [Przetwarzanie obrazów](#przetwarzanie-obrazów)
  - [Biblioteki przydatne przy narzędziach dla CS2](#biblioteki-przydatne-przy-narzędziach-dla-cs2)

---

## SDK i bazowe frameworki

| Repozytorium | Link | Opis |
| --- | --- | --- |
| **bruhmoment21/cs2-sdk** | https://github.com/bruhmoment21/cs2-sdk | SDK/baza dla Counter-Strike 2 napisana w C++. Obsługuje DirectX 11 i Vulkan, systemy Windows oraz Linux. Zawiera mechanizmy hookowania (funchook), disassembler (distorm), interfejs GUI (ImGui) oraz system sygnatur (STB). Licencja MIT. Około 418 gwiazdek. |
| **uraioa/cs2sdk** | https://github.com/uraioa/cs2sdk | Fork projektu cs2-sdk (gałąź v1). Baza SDK w C++ z obsługą ESP, renderowania i RCS (Recoil Control System). |
| **neverlosecc/source2gen** | https://github.com/neverlosecc/source2gen | Automatyczny generator SDK dla gier opartych na silniku Source 2 (CS2, Dota 2, Half-Life: Alyx itd.). Działa na wielu platformach i generuje nagłówki zgodne z C++23, C23 oraz IDA. |
| **neverlosecc/source2sdk** | https://github.com/ccsimplyspolit/CS2-SDK-Reference/tree/main/source2sdk | Wygenerowane SDK Source 2 dla różnych gier. Każda gra znajduje się w osobnej gałęzi (CS2, Dota itp.). |

## Analiza pamięci i generowanie offsetów

| Repozytorium | Link | Opis |
| --- | --- | --- |
| **a2x/cs2-dumper** | https://github.com/a2x/cs2-dumper | Najpopularniejsze narzędzie do generowania offsetów i interfejsów dla CS2 (~2181 gwiazdek, 334 forki). Napisane w Rust z wykorzystaniem memflow. Obsługuje Windows i Linux. Generuje kod dla C#, C++, Rust oraz JSON. |
| **scros22/cs2-universal-offsets** | https://github.com/scros22/cs2-universal-offsets | Generator zewnętrznego SDK dla CS2 napisany w Rust. Odczytuje działający proces cs2.exe i generuje strukturę plików nagłówkowych C++ zawierającą schematy, sygnatury, offsety, interfejsy, tablice wirtualne (vtables) oraz definicje przycisków. Około 70 gwiazdek. |
| **sezzyaep/CS2-OFFSETS** | https://github.com/sezzyaep/CS2-OFFSETS | Gotowe, statyczne offsety i interfejsy dla CS2 w wielu językach (C#, C++, Python, Rust, JSON, YAML). Nie wymaga uruchamiania dumppera — wystarczy pobrać aktualne pliki. Około 194 gwiazdek. |
| **a2x/cs2-analyzer** | https://github.com/a2x/cs2-analyzer | Rozwijana wersja offline projektu cs2-dumper, dostępna również jako demonstracja webowa. |
| **dr-NHA/CS2-Schema-System-Dumper-CE** | https://github.com/dr-NHA/CS2-Schema-System-Dumper-CE | Narzędzie do zrzucania schematów systemowych CS2 oparte na Cheat Engine. |

## Reverse engineering i frameworki badawcze

| Repozytorium | Link | Opis |
| --- | --- | --- |
| **Amiralisa5/Counter-Strike-2-Reverse-Engineering-Framework** | https://github.com/Amiralisa5/Counter-Strike-2-Reverse-Engineering-Framework | Aspasia — framework badawczy w C++ przeznaczony do reverse engineeringu i prototypowania mechanik w CS2. Powstał jako praca magisterska na UC3M. Zawiera moduły do analizy encji, ruchu oraz przykładowe implementacje. |
| **Travers9483/mcp-cheat-engine** | https://github.com/Travers9483/mcp-cheat-engine | Serwer MCP umożliwiający asystentom AI sterowanie Cheat Engine, x64dbg i Ghidrą. Obsługuje skanowanie pamięci, odczyt, zapis, deasemblację i inne operacje przez wspólny interfejs. |

## Narzędzia zewnętrzne i projekty open source

| Repozytorium | Link | Opis |
| --- | --- | --- |
| **RvD-Projects/External-CheatEngine** | https://github.com/RvD-Projects/External-CheatEngine | Projekt w C++ z modułową architekturą, automatyczną aktualizacją offsetów oraz pipeline'ami budowania. |
| **danielkrupinski/Osiris** | https://github.com/danielkrupinski/Osiris | Wieloplatformowy projekt z interfejsem opartym na Panorama UI. |
| **ByteCorum/DragonBurn** | https://github.com/ByteCorum/DragonBurn | Zewnętrzny projekt działający w trybie jądra (kernel-mode), wykorzystujący wyłącznie odczyt pamięci. |
| **IMXNOOBX/cs2-external-esp** | https://github.com/IMXNOOBX/cs2-external-esp | Prosty projekt z nakładką Discord/GDI, zaprojektowany z naciskiem na przejrzystość i wydajność. |
| **Valthrun/valthrun-cs2** | https://github.com/Valthrun/valthrun-cs2 | Projekt wykorzystujący wyłącznie odczyt pamięci w trybie jądra. |
| **avitran0/deadlocked** | https://github.com/avitran0/deadlocked | Projekt przeznaczony wyłącznie dla systemu Linux. |

## Tworzenie serwerów i pluginów

| Repozytorium | Link | Opis |
| --- | --- | --- |
| **roflmuffin/CounterStrikeSharp** | https://github.com/roflmuffin/CounterStrikeSharp | Framework umożliwiający pisanie pluginów serwerowych dla Counter-Strike 2 w języku C#. |
| **antonpup/CounterStrike2GSI** | https://github.com/antonpup/CounterStrike2GSI | Biblioteka C# do komunikacji z systemem Game State Integration (GSI) w CS2. |
| **shobhit-pathak/MatchZy** | https://github.com/shobhit-pathak/MatchZy | Plugin do organizacji treningów, PUG-ów, scrimów i meczów z obsługą Get5. |
| **B3none/cs2-retakes** | https://github.com/B3none/cs2-retakes | Implementacja trybu Retakes dla CS2 oparta na wersji stworzonej wcześniej dla CS:GO. |

## Narzędzia do dem i powtórek

| Repozytorium | Link | Opis |
| --- | --- | --- |
| **markus-wa/demoinfocs-golang** | https://github.com/markus-wa/demoinfocs-golang | Parser dem Counter-Strike 2 napisany w języku Go. |
| **LaihoE/demoparser** | https://github.com/LaihoE/demoparser | Parser powtórek CS2 dostępny dla Pythona i JavaScript. |

## Narzędzia pomocnicze

| Repozytorium | Link | Opis |
| --- | --- | --- |
| **FN-FAL113/cs2-server-picker** | https://github.com/FN-FAL113/cs2-server-picker | Lekki i przenośny selektor serwerów dla CS2 oraz Deadlock. |
| **Jyben/cs2-mm-server-picker** | https://github.com/Jyben/cs2-mm-server-picker | Selektor serwerów matchmakingowych dla Windows i Linux. |
| **JohnTimmermann/JTs-Hud** | https://github.com/JohnTimmermann/JTs-Hud | Menedżer HUD wykorzystujący GSI oraz serwer Node.js z WebSocketami. |
| **drweissbrot/cs-hud** | https://github.com/drweissbrot/cs-hud | Niestandardowy HUD dla widza Counter-Strike. |
| **Flowtter/crispy** | https://github.com/Flowtter/crispy | Platforma ML do automatycznego tworzenia montaży z gier przy użyciu sieci neuronowych wykrywających najciekawsze momenty. |
| **joedwards32/CS2** | https://github.com/joedwards32/CS2 | Obraz Docker dla dedykowanego serwera CS2. |
| **armync/ArminC-AutoExec** | https://github.com/armync/ArminC-AutoExec | Szczegółowo udokumentowany i przeanalizowany plik autoexec dla CS2 bez błędnych konfiguracji. |

## Oficjalne zasoby Valve

| Zasób | Link | Opis |
| --- | --- | --- |
| **CS2 Workshop Tools** | https://developer.valvesoftware.com/wiki/Counter-Strike_2_Workshop_Tools | Oficjalna dokumentacja Valve dotycząca tworzenia modyfikacji do CS2: projektowanie poziomów, skrypty, modele, materiały, efekty cząsteczkowe, Source Filmmaker oraz API skryptowe. |
| **Source SDK 2013** | https://github.com/ValveSoftware/source-sdk-2013 | Oficjalne repozytorium Valve zawierające Source SDK 2013 dla silnika Source 1. |
| **Source-1-Games** | https://github.com/ValveSoftware/Source-1-Games | Oficjalne repozytoria gier opartych na silniku Source 1. |

## Najważniejsze projekty

| Kategoria | Rekomendowany projekt | Dlaczego warto |
| --- | --- | --- |
| Offsety i analiza pamięci | **a2x/cs2-dumper** | Najbardziej rozwijany i najczęściej używany dumper offsetów oraz interfejsów dla CS2 (~2,1 tys. gwiazdek). |
| Generator SDK | **scros22/cs2-universal-offsets** | Automatycznie generuje kompletne nagłówki SDK bez ręcznej analizy. |
| SDK / Framework bazowy | **bruhmoment21/cs2-sdk** | Najpopularniejsza otwartoźródłowa baza do projektów związanych z CS2. |
| Generator SDK Source 2 | **neverlosecc/source2gen** | Uniwersalne narzędzie do generowania nagłówków SDK dla wielu gier opartych na silniku Source 2. |

---

## Biblioteki C++ do efektów

Ogólne, uniwersalne biblioteki C++ do grafiki, dźwięku i przetwarzania obrazu — przydatne w wielu projektach, niekoniecznie związanych z CS2.

### Renderowanie i grafika

| Biblioteka | Link | Opis |
| --- | --- | --- |
| **OpenGL** | https://www.khronos.org/opengl/ | Wieloplatformowe API do renderowania grafiki 2D i 3D. De facto standard dla grafiki akcelerowanej przez GPU. |
| **DirectX 11/12** | https://learn.microsoft.com/en-us/windows/win32/directx | API graficzne firmy Microsoft dla systemu Windows. |
| **Vulkan** | https://www.khronos.org/vulkan/ | Nowoczesne, wieloplatformowe API graficzne o niskim narzucie z bezpośrednią kontrolą nad GPU. |
| **SDL2** | https://www.libsdl.org/ | Wieloplatformowa biblioteka do obsługi okien, wejścia użytkownika oraz grafiki. |
| **SFML** | https://www.sfml-dev.org/ | Obiektowa biblioteka C++ oparta na OpenGL do obsługi grafiki, okien, dźwięku i sieci. |
| **GLFW** | https://www.glfw.org/ | Lekka biblioteka do tworzenia okien z kontekstem OpenGL. |
| **Dear ImGui** | https://github.com/ocornut/imgui | Biblioteka GUI typu Immediate Mode dla C++. Obsługuje OpenGL, DirectX i Vulkan. |
| **bgfx** | https://github.com/bkaradzic/bgfx | Wieloplatformowa biblioteka renderująca, ujednolicająca obsługę OpenGL, DirectX, Vulkan oraz Metal. |
| **Magnum** | https://magnum.graphics/ | Lekki i modułowy silnik graficzny C++11 do aplikacji 2D i 3D. |
| **Ogre3D** | https://ogre3d.org/ | Silnik grafiki 3D oparty na scenach z elastyczną architekturą wtyczek. |

### Systemy cząsteczek

| Biblioteka | Link | Opis |
| --- | --- | --- |
| **ParticleUniverse** | https://github.com/ParticleUniverse/ParticleUniverse | Otwartoźródłowy silnik systemów cząsteczkowych dla Ogre3D — ogień, dym, eksplozje itp. |

### Systemy shaderów

| Biblioteka | Link | Opis |
| --- | --- | --- |
| **GLSL** | https://www.khronos.org/opengl/wiki/OpenGL_Shading_Language | Wysokopoziomowy język shaderów dla OpenGL. |
| **HLSL** | https://learn.microsoft.com/en-us/windows/win32/direct3dhlsl/dx-graphics-hlsl | Język shaderów firmy Microsoft dla DirectX. |
| **SPIR-V** | https://www.khronos.org/spirv/ | Pośredni format shaderów wykorzystywany przez Vulkan i OpenGL. |
| **ShaderConductor** | https://github.com/microsoft/ShaderConductor | Narzędzie Microsoftu do kompilacji shaderów pomiędzy różnymi API. |
| **OptiX** | https://developer.nvidia.com/optix | Silnik ray tracingu firmy NVIDIA z API C++. |

### Efekty dźwiękowe

| Biblioteka | Link | Opis |
| --- | --- | --- |
| **OpenAL** | https://www.khronos.org/openal/ | Wieloplatformowe API dźwięku 3D. |
| **OpenAL Soft** | https://openal-soft.org/ | Otwartoźródłowa implementacja OpenAL z obsługą HRTF. |
| **miniaudio** | https://github.com/mackron/miniaudio | Bardzo lekka biblioteka C do odtwarzania i nagrywania dźwięku w jednym pliku źródłowym. |
| **SDL_mixer** | https://www.libsdl.org/projects/SDL_mixer/ | Biblioteka do miksowania dźwięku oparta na SDL2. |
| **FMOD** | https://www.fmod.com/ | Profesjonalny silnik audio do gier z API C++. Darmowy dla projektów niezależnych. |
| **Wwise** | https://www.audiokinetic.com/products/wise/ | Profesjonalne middleware audio wykorzystywane w produkcjach AAA. |
| **RtAudio** | https://www.music.mcgill.ca/~gary/rtaudio/ | Biblioteka C++ do wejścia i wyjścia audio w czasie rzeczywistym. |
| **JUCE** | https://juce.com/ | Framework C++ do tworzenia aplikacji audio i wtyczek VST, AU oraz AAX. |
| **SoundTouch** | https://www.surina.net/soundtouch/ | Biblioteka do zmiany tempa odtwarzania i wysokości dźwięku bez utraty jakości. |
| **libsndfile** | https://libsndfile.github.io/libsndfile/ | Biblioteka do odczytu i zapisu plików audio (WAV, AIFF, FLAC i inne). |
| **PortAudio** | http://www.portaudio.com/ | Wieloplatformowa biblioteka C do obsługi wejścia i wyjścia audio. |

### Przetwarzanie obrazów

| Biblioteka | Link | Opis |
| --- | --- | --- |
| **OpenCV** | https://opencv.org/ | Najpopularniejsza biblioteka C++ do przetwarzania obrazu. Zawiera ponad 2500 algorytmów. |
| **stb_image** | https://github.com/nothings/stb | Jednoplikowa biblioteka do wczytywania obrazów (PNG, JPEG, BMP, TGA itd.). |
| **stb_image_write** | https://github.com/nothings/stb | Jednoplikowa biblioteka do zapisywania obrazów (PNG, JPEG, BMP). |
| **FreeImage** | http://freeimage.sourceforge.net/ | Otwartoźródłowa biblioteka do odczytu i zapisu wielu formatów obrazów. |
| **libpng** | http://www.libpng.org/pub/png/libpng.html | Biblioteka do obsługi plików PNG. |
| **libjpeg** | http://www.ijg.org/ | Biblioteka do odczytu i zapisu plików JPEG. |
| **OpenEXR** | https://openexr.com/ | Biblioteka do obsługi obrazów HDR w formacie OpenEXR. |
| **Magick++** | https://imagemagick.org/script/index.php | Interfejs C++ dla ImageMagick obsługujący ponad 200 formatów obrazów. |
| **CImg** | http://cimg.eu/ | Lekka biblioteka szablonowa C++ do przetwarzania obrazów. |
| **Boost.GIL** | https://www.boost.org/doc/libs/release/libs/gil/ | Framework do przetwarzania obrazów będący częścią biblioteki Boost. |
| **Halide** | https://halide-lang.org/ | Język i kompilator przeznaczony do wydajnego przetwarzania obrazów oraz zastosowań AI. |
| **Intel IPP** | https://www.intel.com/content/www/us/en/developer/tools/oneapi/ipp.html | Zoptymalizowana biblioteka C/C++ do przetwarzania obrazów i sygnałów na procesorach Intel. |

### Biblioteki przydatne przy narzędziach dla CS2

Kontekst: projekty wykorzystujące Present Hook, nakładki (overlay), analizę pamięci lub własny interfejs.

| Biblioteka | Link | Zastosowanie |
| --- | --- | --- |
| **Dear ImGui** | https://github.com/ocornut/imgui | Tworzenie menu i interfejsów nakładek (overlay). Wykorzystywana m.in. w cs2-sdk i wielu projektach open source. |
| **funchook** | https://github.com/kubo/funchook | Biblioteka do hookowania funkcji (np. Present w DirectX 11 lub Vulkan). |
| **distorm** | https://github.com/gdabah/distorm | Disassembler x86/x64 wykorzystywany do analizy kodu oraz wyszukiwania sygnatur. |
| **memflow** | https://github.com/memflow/memflow | Wieloplatformowy framework do odczytu pamięci używany m.in. przez cs2-dumper. |
| **OpenCV** | https://opencv.org/ | Przetwarzanie obrazów, konwersja kolorów, wykrywanie konturów oraz analiza obrazu. |
| **stb_image** | https://github.com/nothings/stb | Wczytywanie tekstur do interfejsów użytkownika i innych elementów graficznych. |
| **OpenGL** | https://www.khronos.org/opengl/ | Popularne API renderujące wykorzystywane do tworzenia aplikacji graficznych i nakładek. |
| **Vulkan** | https://www.khronos.org/vulkan/ | Nowoczesne API graficzne przydatne przy projektach wykorzystujących Vulkan jako backend renderujący. |
| **SDL2** | https://www.libsdl.org/ | Obsługa okien, wejścia użytkownika i podstaw aplikacji wieloplatformowych. |
| **miniaudio** | https://github.com/mackron/miniaudio | Lekka biblioteka audio do własnych narzędzi oraz aplikacji C++. |

---

## Licencja / Uwaga

Ten dokument to jedynie zestawienie linków do publicznie dostępnych repozytoriów i bibliotek. Każdy projekt ma własną licencję — sprawdź ją przed użyciem. Linki do narzędzi typu "external cheat" / dumper offsetów są tu wymienione w celach informacyjnych (reverse engineering, badania nad silnikiem Source 2); korzystanie z nich w grze online może naruszać regulamin Valve/VAC.
