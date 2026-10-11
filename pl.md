# awesome-cs2-dev-resources

Zbiór repozytoriów GitHub, dokumentacji i bibliotek C++ przydatnych przy tworzeniu narzędzi oraz analizie gier opartych na silniku Source 2, w szczególności Counter-Strike 2 (CS2).

Lista obejmuje SDK, generatory struktur i offsetów, narzędzia do analizy plików binarnych, frameworki badawcze, pluginy serwerowe, parsery dem, narzędzia pomocnicze oraz biblioteki do grafiki, dźwięku i przetwarzania obrazów.

> **Cel repozytorium:** katalog informacyjny i edukacyjny. Obecność projektu na liście nie oznacza rekomendacji jego używania, potwierdzenia bezpieczeństwa ani gwarancji zgodności z aktualną wersją gry.

## Spis treści

- [SDK i frameworki bazowe](#sdk-i-frameworki-bazowe)
- [Analiza plików, schematów i offsetów](#analiza-plików-schematów-i-offsetów)
- [Reverse engineering i frameworki badawcze](#reverse-engineering-i-frameworki-badawcze)
- [Projekty społecznościowe](#projekty-społecznościowe)
- [Serwery i pluginy](#serwery-i-pluginy)
- [Dema i powtórki](#dema-i-powtórki)
- [Narzędzia pomocnicze](#narzędzia-pomocnicze)
- [Oficjalne zasoby Valve](#oficjalne-zasoby-valve)
- [Polecane punkty startowe](#polecane-punkty-startowe)
- [Biblioteki C++](#biblioteki-c)
  - [Grafika i renderowanie](#grafika-i-renderowanie)
  - [Systemy cząsteczek](#systemy-cząsteczek)
  - [Shadery](#shadery)
  - [Dźwięk](#dźwięk)
  - [Przetwarzanie obrazów](#przetwarzanie-obrazów)
  - [Biblioteki przydatne przy narzędziach CS2](#biblioteki-przydatne-przy-narzędziach-cs2)
  - [Narzędzia ogólnego zastosowania](#narzędzia-ogólnego-zastosowania)
- [Licencje i bezpieczeństwo](#licencje-i-bezpieczeństwo)

---

## SDK i frameworki bazowe

| Projekt | Link | Opis |
|---|---|---|
| **bruhmoment21/cs2-sdk** | [GitHub](https://github.com/bruhmoment21/cs2-sdk) | Baza SDK w C++ do eksperymentów z CS2. Projekt opisuje obsługę Windows i Linux oraz backendów graficznych DirectX 11 i Vulkan. Sprawdź README i licencję przed użyciem. |
| **uraioa/cs2sdk** | [GitHub](https://github.com/uraioa/cs2sdk) | Starsza wersja lub fork bazy SDK dla CS2. Zachowano pozycję z oryginalnej listy; sprawdź zgodność z aktualną wersją gry. |
| **neverlosecc/source2gen** | [GitHub](https://github.com/neverlosecc/source2gen) | Generator SDK dla gier opartych na Source 2. Przed wykorzystaniem sprawdź obsługiwane gry, formaty wyjściowe i wymagania wersji. |
| **CS2-SDK-Reference/source2sdk** | [GitHub — katalog source2sdk](https://github.com/ccsimplyspolit/CS2-SDK-Reference/tree/main/source2sdk) | Zbiór referencyjnych plików SDK. Uwaga: ten link prowadzi do katalogu w repozytorium `CS2-SDK-Reference`, a nie do repozytorium `neverlosecc/source2sdk`. |

## Analiza plików, schematów i offsetów

| Projekt | Link | Opis |
|---|---|---|
| **a2x/cs2-dumper** | [GitHub](https://github.com/a2x/cs2-dumper) | Narzędzie napisane w Rust do generowania informacji o strukturach, offsetach i interfejsach związanych z CS2. Wyniki mogą wymagać aktualizacji po zmianach gry. |
| **scros22/cs2-universal-offsets** | [GitHub](https://github.com/scros22/cs2-universal-offsets) | Projekt w Rust związany z generowaniem danych SDK i struktur dla CS2. Sprawdź dokumentację dotyczącą sposobu odczytu danych i obsługiwanych wersji. |
| **sezzyaep/CS2-OFFSETS** | [GitHub](https://github.com/sezzyaep/CS2-OFFSETS) | Zestaw gotowych definicji offsetów i interfejsów. Aktualność danych zależy od zmian w grze. |
| **a2x/cs2-analyzer** | [GitHub](https://github.com/a2x/cs2-analyzer) · [Demo webowe](https://a2x.github.io/cs2-analyzer) | Biblioteka/narzędzie w Rust do analizowania plików binarnych CS2, zarówno z dysku, jak i załadowanych do pamięci. |
| **dr-NHA/CS2-Schema-System-Dumper-CE** | [GitHub](https://github.com/dr-NHA/CS2-Schema-System-Dumper-CE) | Narzędzie oparte na Cheat Engine do zrzucania informacji o systemie schematów CS2. Sprawdź wymagania i stan projektu w repozytorium. |

> **Ważne:** offsety i wygenerowane struktury nie są stabilnym API. Nie zakładaj, że dane z poprzedniej aktualizacji gry będą nadal prawidłowe.

## Reverse engineering i frameworki badawcze

| Projekt | Link | Opis |
|---|---|---|
| **Amiralisa5/Counter-Strike-2-Reverse-Engineering-Framework** | [GitHub](https://github.com/Amiralisa5/Counter-Strike-2-Reverse-Engineering-Framework) | Aspasia — framework badawczy w C++ do eksperymentów z mechanikami CS2 i analizy działania gry. Powstał w ramach pracy magisterskiej na Universidad Carlos III de Madrid. Projekt ma charakter badawczy, ale jego techniki mogą zostać wykorzystane również do manipulowania grą. |
| **Travers9483/mcp-cheat-engine** | [GitHub](https://github.com/Travers9483/mcp-cheat-engine) | Serwer MCP łączący asystenta AI z narzędziami do reverse engineeringu, takimi jak Cheat Engine, x64dbg i Ghidra. Nie jest to SDK CS2, lecz ogólne narzędzie do analizy i debugowania. |

## Projekty społecznościowe

Poniższe projekty są nieoficjalnymi narzędziami społeczności. Ich obecność w katalogu nie oznacza rekomendacji używania ich podczas gry online.

| Projekt | Link | Opis |
|---|---|---|
| **RvD-Projects/External-CheatEngine** | [GitHub](https://github.com/RvD-Projects/External-CheatEngine) | Zewnętrzny projekt związany z analizą i modyfikowaniem działania CS2. Przed użyciem sprawdź aktualność kodu, licencję i wymagania. |
| **danielkrupinski/Osiris** | [GitHub](https://github.com/danielkrupinski/Osiris) | Projekt dla CS2 z interfejsem opartym na Panorama UI. Repozytorium opisuje obsługę Windows i Linux. |
| **ByteCorum/DragonBurn** | [GitHub](https://github.com/ByteCorum/DragonBurn) | Zewnętrzny projekt związany z odczytem pamięci w trybie jądra. README projektu wskazuje, że jego stan techniczny może się zmieniać; sprawdź aktualne informacje przed oceną użyteczności. |
| **IMXNOOBX/cs2-external-esp** | [GitHub](https://github.com/IMXNOOBX/cs2-external-esp) | Zewnętrzna nakładka ESP dla CS2. Repozytorium opisuje nowszą przebudowaną wersję z automatycznym skanowaniem offsetów. |
| **Valthrun/valthrun-cs2** | [GitHub](https://github.com/Valthrun/valthrun-cs2) · [Strona pobierania](https://valth.run/download) | Otwarty projekt zewnętrzny oparty na odczycie danych gry w trybie jądra. Repozytorium nadal jest dostępne; według informacji w wydaniach pliki binarne nie są już udostępniane przez GitHub, a pobieranie przekierowano na stronę projektu. |
| **avitran0/deadlocked** | [GitHub](https://github.com/avitran0/deadlocked) | Projekt dla Linuxa związany z zewnętrzną analizą stanu CS2. Obsługa zależy od konfiguracji systemu i środowiska graficznego; część funkcji może wpływać na pamięć gry i stwarzać ryzyko blokady konta. |

## Serwery i pluginy

| Projekt | Link | Opis |
|---|---|---|
| **roflmuffin/CounterStrikeSharp** | [GitHub](https://github.com/roflmuffin/CounterStrikeSharp) · [Dokumentacja](https://docs.cssharp.dev/) | Framework do tworzenia pluginów serwerowych dla CS2 w C#. Wykorzystuje .NET i Metamod:Source. |
| **antonpup/CounterStrike2GSI** | [GitHub](https://github.com/antonpup/CounterStrike2GSI) | Biblioteka C# związana z integracją Game State Integration. Sprawdź zgodność z aktualnym formatem danych CS2. |
| **shobhit-pathak/MatchZy** | [GitHub](https://github.com/shobhit-pathak/MatchZy) · [Dokumentacja](https://shobhit-pathak.github.io/MatchZy/) | Plugin do zarządzania treningami, PUG-ami, scrimami i meczami. Obsługuje konfiguracje meczów oraz integrację z ekosystemem Get5. |
| **B3none/cs2-retakes** | [GitHub](https://github.com/B3none/cs2-retakes) | Implementacja trybu Retakes dla CS2, napisana w C# i oparta na wcześniejszym projekcie dla CS:GO. |

## Dema i powtórki

| Projekt | Link | Opis |
|---|---|---|
| **markus-wa/demoinfocs-golang** | [GitHub](https://github.com/markus-wa/demoinfocs-golang) | Parser dem Counter-Strike napisany w Go. Repozytorium zawiera wydania oraz informacje o obsługiwanych wersjach formatu. |
| **LaihoE/demoparser** | [GitHub](https://github.com/LaihoE/demoparser) | Parser dem CS2 z interfejsami dla języków i środowisk programistycznych, w tym Pythona i JavaScript. Sprawdź README w sprawie bieżącego API. |

## Narzędzia pomocnicze

| Projekt | Link | Opis |
|---|---|---|
| **FN-FAL113/cs2-server-picker** | [GitHub](https://github.com/FN-FAL113/cs2-server-picker) | Narzędzie do wyboru serwerów dla CS2 i innych obsługiwanych gier. Sprawdź, czy bieżąca wersja nadal obsługuje Twoją wersję gry. |
| **Jyben/cs2-mm-server-picker** | [GitHub](https://github.com/Jyben/cs2-mm-server-picker) | Selektor serwerów matchmakingowych. Przed instalacją sprawdź obsługiwane systemy i zgodność z aktualnym klientem gry. |
| **JohnTimmermann/JTs-Hud** | [GitHub](https://github.com/JohnTimmermann/JTs-Hud) | Niestandardowy HUD wykorzystujący dane GSI i technologie webowe. |
| **drweissbrot/cs-hud** | [GitHub](https://github.com/drweissbrot/cs-hud) | Niestandardowy HUD przeznaczony do prezentowania informacji związanych z Counter-Strike. |
| **Flowtter/crispy** | [GitHub](https://github.com/Flowtter/crispy) | Projekt wykorzystujący uczenie maszynowe do analizy materiałów z gier i automatyzacji tworzenia montaży. Sprawdź aktualny opis oraz wymagania repozytorium. |
| **joedwards32/CS2** | [GitHub](https://github.com/joedwards32/CS2) | Obraz Docker i narzędzia do uruchamiania dedykowanego serwera CS2. |
| **armync/ArminC-AutoExec** | [GitHub](https://github.com/armync/ArminC-AutoExec) | Przykładowy, udokumentowany plik konfiguracji autoexec dla CS2. Przy aktualizacjach gry warto sprawdzać, czy komendy nadal działają. |

## Oficjalne zasoby Valve

| Zasób | Link | Opis |
|---|---|---|
| **CS2 Workshop Tools** | [Dokumentacja Valve Developer Community](https://developer.valvesoftware.com/wiki/Counter-Strike_2_Workshop_Tools) | Dokumentacja narzędzi warsztatowych CS2, w tym tworzenia map, materiałów, modeli i innych zasobów. |
| **Source SDK 2013** | [GitHub](https://github.com/ValveSoftware/source-sdk-2013) | Oficjalne SDK dla silnika Source 1. **Nie jest to SDK silnika Source 2 używanego przez CS2.** |
| **Source-1-Games** | [GitHub](https://github.com/ValveSoftware/Source-1-Games) | Oficjalne repozytoria gier opartych na Source 1. Przydatne jako materiał porównawczy, nie jako bezpośrednie SDK CS2. |

## Polecane punkty startowe

Poniższe pozycje są podzielone według zastosowania. To propozycje punktów startowych, a nie ranking popularności.

| Zastosowanie | Projekt | Dlaczego warto zacząć tutaj |
|---|---|---|
| Analiza plików binarnych | [a2x/cs2-analyzer](https://github.com/a2x/cs2-analyzer) | Projekt skupiony na analizie binariów CS2. |
| Generowanie danych i offsetów | [a2x/cs2-dumper](https://github.com/a2x/cs2-dumper) | Punkt wyjścia do badania struktur i danych zmieniających się wraz z aktualizacjami gry. |
| SDK i eksperymenty w C++ | [bruhmoment21/cs2-sdk](https://github.com/bruhmoment21/cs2-sdk) | Przykład bazy SDK dla CS2. |
| Generowanie SDK Source 2 | [neverlosecc/source2gen](https://github.com/neverlosecc/source2gen) | Generator przeznaczony dla gier opartych na Source 2. |
| Pluginy serwerowe | [CounterStrikeSharp](https://github.com/roflmuffin/CounterStrikeSharp) | Framework do pisania pluginów w C#. |
| Parsowanie dem w Go | [demoinfocs-golang](https://github.com/markus-wa/demoinfocs-golang) | Biblioteka do analizy danych zapisanych w demach. |
| Parsowanie dem w Pythonie/JavaScript | [demoparser](https://github.com/LaihoE/demoparser) | Alternatywa dla narzędzi napisanych w Go. |

---

# Biblioteki C++

Poniższe biblioteki są ogólnego zastosowania. Nie wszystkie są bezpośrednio związane z CS2 — mogą być przydatne przy tworzeniu narzędzi, wizualizacji danych, aplikacji desktopowych, przetwarzaniu mediów i prototypowaniu.

## Grafika i renderowanie

| Biblioteka/API | Link | Opis |
|---|---|---|
| **OpenGL** | [Strona Khronos](https://www.khronos.org/opengl/) | Wieloplatformowe API do renderowania grafiki 2D i 3D. |
| **DirectX 11/12** | [Microsoft Learn](https://learn.microsoft.com/en-us/windows/win32/directx) | Zestaw API graficznych i multimedialnych firmy Microsoft dla Windows. |
| **Vulkan** | [Strona Khronos](https://www.khronos.org/vulkan/) | Wieloplatformowe API graficzne o niskim narzucie i jawniejszym zarządzaniu zasobami GPU. |
| **SDL** | [Strona SDL](https://www.libsdl.org/) · [GitHub](https://github.com/libsdl-org/SDL) | Biblioteka do obsługi okien, wejścia użytkownika, kontrolerów i funkcji multimedialnych. |
| **SFML** | [Strona SFML](https://www.sfml-dev.org/) | Biblioteka C++ do obsługi grafiki, okien, dźwięku i sieci. |
| **GLFW** | [Strona GLFW](https://www.glfw.org/) | Biblioteka do tworzenia okien i kontekstów OpenGL oraz Vulkan. |
| **Dear ImGui** | [GitHub](https://github.com/ocornut/imgui) | Biblioteka GUI typu Immediate Mode dla C++. Obsługuje różne backendy renderowania. |
| **bgfx** | [GitHub](https://github.com/bkaradzic/bgfx) | Wieloplatformowa biblioteka renderująca z abstrakcją nad różnymi API graficznymi. |
| **Magnum** | [Strona projektu](https://magnum.graphics/) · [GitHub](https://github.com/mosra/magnum) | Modułowy framework C++ do grafiki i aplikacji 2D/3D. |
| **OGRE** | [Strona projektu](https://ogre3d.org/) · [GitHub](https://github.com/OGRECave/ogre) | Silnik renderowania 3D z architekturą opartą na scenach. |

## Systemy cząsteczek

| Biblioteka | Link | Opis |
|---|---|---|
| **Particle Universe** | [GitHub](https://github.com/ParticleUniverse/ParticleUniverse) | System cząsteczek przeznaczony dla OGRE. Przed użyciem sprawdź zgodność z wybraną wersją silnika. |

## Shadery

| Technologia | Link | Opis |
|---|---|---|
| **GLSL** | [Dokumentacja Khronos](https://www.khronos.org/opengl/wiki/OpenGL_Shading_Language) | Język shaderów używany przede wszystkim z OpenGL. |
| **HLSL** | [Microsoft Learn](https://learn.microsoft.com/en-us/windows/win32/direct3dhlsl/dx-graphics-hlsl) | Język shaderów firmy Microsoft, wykorzystywany w ekosystemie DirectX. |
| **SPIR-V** | [Strona Khronos](https://www.khronos.org/spirv/) | Pośrednia reprezentacja shaderów wykorzystywana m.in. w Vulkanie. |
| **ShaderConductor** | [GitHub](https://github.com/microsoft/ShaderConductor) | Narzędzie Microsoftu do translacji i kompilacji shaderów pomiędzy różnymi językami i backendami. Sprawdź bieżący status projektu. |
| **NVIDIA OptiX** | [Strona NVIDIA](https://developer.nvidia.com/optix) | API do akcelerowanego ray tracingu na obsługiwanych GPU NVIDIA. |

## Dźwięk

| Biblioteka | Link | Opis |
|---|---|---|
| **OpenAL** | [Strona Khronos](https://www.khronos.org/openal/) | API do przestrzennego odtwarzania dźwięku. |
| **OpenAL Soft** | [Strona projektu](https://openal-soft.org/) · [GitHub](https://github.com/kcat/openal-soft) | Otwarta implementacja OpenAL, oferująca m.in. obsługę HRTF. |
| **miniaudio** | [GitHub](https://github.com/mackron/miniaudio) | Lekka biblioteka audio w C, dostępna w formie plików źródłowych. |
| **SDL_mixer** | [GitHub](https://github.com/libsdl-org/SDL_mixer) | Biblioteka miksowania i odtwarzania dźwięku z ekosystemu SDL. |
| **FMOD** | [Strona FMOD](https://www.fmod.com/) | Silnik audio do gier z API dla języka C/C++ i innych środowisk. Warunki licencji zależą od zastosowania. |
| **Audiokinetic Wwise** | [Strona Wwise](https://www.audiokinetic.com/en/wwise/) | Middleware audio wykorzystywane w produkcji gier. Sprawdź aktualne warunki licencji. |
| **RtAudio** | [GitHub](https://github.com/thestk/rtaudio) | Biblioteka C++ do wejścia i wyjścia audio w czasie rzeczywistym. |
| **JUCE** | [Strona JUCE](https://juce.com/) | Framework C++ do tworzenia aplikacji audio, narzędzi i wtyczek. Sprawdź warunki licencyjne. |
| **SoundTouch** | [Strona projektu](https://www.surina.net/soundtouch/) · [GitHub](https://github.com/rspeyer/soundtouch) | Biblioteka do zmiany tempa i wysokości dźwięku. |
| **libsndfile** | [Strona projektu](https://libsndfile.github.io/libsndfile/) · [GitHub](https://github.com/libsndfile/libsndfile) | Biblioteka do odczytu i zapisu popularnych formatów plików audio. |
| **PortAudio** | [Strona projektu](https://www.portaudio.com/) · [GitHub](https://github.com/PortAudio/portaudio) | Wieloplatformowa biblioteka C do obsługi wejścia i wyjścia audio. |

## Przetwarzanie obrazów

| Biblioteka | Link | Opis |
|---|---|---|
| **OpenCV** | [Strona OpenCV](https://opencv.org/) · [GitHub](https://github.com/opencv/opencv) | Biblioteka do przetwarzania obrazów, wizji komputerowej i analizy wideo. |
| **stb_image** | [GitHub — stb](https://github.com/nothings/stb) | Jednoplikowa biblioteka do wczytywania wielu popularnych formatów obrazów. |
| **stb_image_write** | [GitHub — stb](https://github.com/nothings/stb) | Jednoplikowa biblioteka do zapisywania obrazów. Jest częścią tego samego repozytorium `stb`. |
| **FreeImage** | [Strona projektu](https://freeimage.sourceforge.io/) | Biblioteka do odczytu i zapisu różnych formatów obrazów. Sprawdź stan utrzymania i licencję przed użyciem. |
| **libpng** | [Strona projektu](http://www.libpng.org/pub/png/libpng.html) · [GitHub](https://github.com/pnggroup/libpng) | Biblioteka do odczytu i zapisu plików PNG. |
| **libjpeg / libjpeg-turbo** | [IJG](https://www.ijg.org/) · [GitHub — libjpeg-turbo](https://github.com/libjpeg-turbo/libjpeg-turbo) | Biblioteki do kodowania i dekodowania JPEG. libjpeg-turbo to odrębna implementacja zoptymalizowana pod kątem wydajności. |
| **OpenEXR** | [Strona OpenEXR](https://openexr.com/) · [GitHub](https://github.com/AcademySoftwareFoundation/openexr) | Format i biblioteki do obrazów HDR, popularne w grafice komputerowej i efektach wizualnych. |
| **ImageMagick / Magick++** | [Strona ImageMagick](https://imagemagick.org/) · [Dokumentacja Magick++](https://imagemagick.org/script/magick++.php) | Narzędzia do konwersji i przetwarzania obrazów; Magick++ udostępnia interfejs C++. |
| **CImg** | [Strona CImg](https://cimg.eu/) · [GitHub](https://github.com/GreycLab/CImg) | Biblioteka C++ do przetwarzania obrazów, wizualizacji i obliczeń numerycznych. |
| **Boost.GIL** | [Dokumentacja](https://www.boost.org/doc/libs/release/libs/gil/) | Biblioteka szablonowa do przetwarzania obrazów będąca częścią Boost. |
| **Halide** | [Strona Halide](https://halide-lang.org/) · [GitHub](https://github.com/halide/Halide) | Język i kompilator do optymalizacji potoków przetwarzania obrazów. |
| **Intel oneAPI IPP** | [Strona Intel IPP](https://www.intel.com/content/www/us/en/developer/tools/oneapi/ipp.html) | Zoptymalizowane funkcje do przetwarzania sygnałów i obrazów. Sprawdź obsługiwane platformy i warunki dystrybucji. |

## Biblioteki przydatne przy narzędziach CS2

W tej sekcji znajdują się biblioteki ogólnego zastosowania, które mogą być pomocne przy tworzeniu aplikacji diagnostycznych, interfejsów, analizatorów plików i narzędzi deweloperskich.

| Biblioteka | Link | Zastosowanie |
|---|---|---|
| **Dear ImGui** | [GitHub](https://github.com/ocornut/imgui) | Interfejsy narzędzi developerskich, debugowania i wizualizacji danych. |
| **funchook** | [GitHub](https://github.com/kubo/funchook) | Biblioteka do przechwytywania wywołań funkcji w celach diagnostycznych i badawczych. Hookowanie może powodować problemy ze stabilnością i kompatybilnością. |
| **distorm** | [GitHub](https://github.com/gdabah/distorm) | Dekoder instrukcji x86/x64 przydatny w analizie kodu maszynowego. Sprawdź stan utrzymania projektu. |
| **memflow** | [GitHub](https://github.com/memflow/memflow) | Framework w Rust do pracy z pamięcią i źródłami danych pamięciowymi. Zakres funkcji zależy od użytych konektorów i konfiguracji. |
| **OpenCV** | [Strona OpenCV](https://opencv.org/) | Przetwarzanie obrazów, analiza klatek wideo i wizja komputerowa. |
| **stb_image** | [GitHub](https://github.com/nothings/stb) | Wczytywanie obrazów i tekstur w aplikacjach. |
| **OpenGL** | [Strona Khronos](https://www.khronos.org/opengl/) | Renderowanie grafiki w aplikacjach wieloplatformowych. |
| **Vulkan** | [Strona Khronos](https://www.khronos.org/vulkan/) | Renderowanie z użyciem nowoczesnego API graficznego. |
| **SDL** | [Strona SDL](https://www.libsdl.org/) | Okna, wejście, kontrolery i podstawowe funkcje aplikacji wieloplatformowych. |
| **miniaudio** | [GitHub](https://github.com/mackron/miniaudio) | Odtwarzanie i nagrywanie dźwięku w narzędziach i aplikacjach. |

## Narzędzia ogólnego zastosowania

Przydatne przy budowaniu większych projektów C++ niezależnie od tego, czy są powiązane z CS2.

| Narzędzie / biblioteka | Link | Opis |
|---|---|---|
| **GLM** | [GitHub](https://github.com/g-truc/glm) | Biblioteka matematyczna C++ inspirowana GLSL; wektory, macierze i operacje geometryczne. |
| **fmt** | [GitHub](https://github.com/fmtlib/fmt) | Wydajne formatowanie tekstu dla C++. |
| **spdlog** | [GitHub](https://github.com/gabime/spdlog) | Biblioteka logowania dla C++. |
| **nlohmann/json** | [GitHub](https://github.com/nlohmann/json) | Biblioteka JSON dla C++, często używana do konfiguracji i wymiany danych. |
| **CMake** | [Strona CMake](https://cmake.org/) · [GitHub](https://github.com/Kitware/CMake) | System konfiguracji i generowania kompilacji dla projektów wieloplatformowych. |
| **vcpkg** | [GitHub](https://github.com/microsoft/vcpkg) | Menedżer pakietów C/C++ od Microsoftu. |
| **libjpeg-turbo** | [GitHub](https://github.com/libjpeg-turbo/libjpeg-turbo) | Wydajna implementacja kodowania i dekodowania JPEG. |

---

## Licencje i bezpieczeństwo

- Każdy projekt ma własną licencję. Sprawdź plik `LICENSE` oraz ewentualne dodatkowe warunki przed użyciem, modyfikacją lub redystrybucją.
- Obecność repozytorium w tym zestawieniu **nie oznacza**, że jego kod został poddany audytowi bezpieczeństwa.
- Nie zakładaj, że projekt nadal działa po aktualizacji CS2. Struktury, offsety, interfejsy i formaty plików mogą ulegać zmianom.
- Niektóre narzędzia do odczytu pamięci, modyfikowania gry lub ingerowania w jej działanie mogą naruszać regulamin Valve i prowadzić do blokady konta.
- Szczególną ostrożność zachowaj przy projektach wymagających sterowników jądra, wyłączania zabezpieczeń systemowych lub uruchamiania plików binarnych pobranych z nieznanych źródeł.
- Nie wyłączaj mechanizmów bezpieczeństwa systemu tylko po to, aby uruchomić nieznane narzędzie.
- Oficjalna dokumentacja Valve i biblioteki ogólnego zastosowania są odrębną kategorią od nieoficjalnych projektów ingerujących w działanie gry.

## Zgłaszanie poprawek

Celem tego zestawienia jest zachowanie użytecznych zasobów technicznych, a nie tworzenie rankingu projektów ani gwarantowanie ich aktualności.
