# Bascanka

**Bascanka** is a free and open-source text editor for Windows designed as a modern, lightweight alternative to traditional editors. It supports a wide range of programming and markup languages and is distributed under the GNU General Public License Version 3.

Built entirely from scratch in **C#** on **.NET 10**, Bascanka is engineered for performance, portability, and simplicity. It runs as a single self-contained executable with no third-party dependencies - just copy and run. Its architecture is optimized for responsiveness even when working with extremely large files, including datasets and logs in the multi-gigabyte range (10 GB and beyond).

Bascanka focuses on efficient resource usage and fast text processing while maintaining a clean, practical editing experience. By minimizing overhead and avoiding unnecessary dependencies, it delivers high performance with a small footprint - making it suitable for both everyday editing and demanding large-file workloads.

## Features

- Supports large text files (10 GB+)
- Syntax highlighting for common languages (C#, JavaScript, Python, HTML, CSS, JSON, XML, and more)
- Hex editor
- Find & replace with regex support
- Column (Box) Selection Mode
- Macro recording and playback
- Tab-based editing
- Word wrap
- Multilanguage UI (English and Croatian built-in, extensible via JSON)
- Theming support

## Build as single exe

#### Self-contained single EXE (includes .NET 10 runtime / ~120 MB exe)
```
dotnet publish "src\Bascanka.App\Bascanka.App.csproj" -c Release -r win-x64 -p:PublishSingleFile=true -p:SelfContained=true
```
#### Framework-dependent single EXE (requires .NET 10 runtime installed / ~2 MB exe)
```
dotnet publish "src\Bascanka.App\Bascanka.App.csproj" -c Release -r win-x64 -p:PublishSingleFile=true -p:SelfContained=false
```

## Run

```
dotnet run --project src/Bascanka.App/Bascanka.App.csproj
```

## Project Structure

```
src/
  Bascanka.Core/          # Text buffer (piece table), search engine, commands
  Bascanka.Editor/        # Editor controls, gutter, tabs, panels, themes
  Bascanka.Plugins.Api/   # Plugin interfaces
  Bascanka.App/           # WinForms application, menus, localization
```

## About the Name

The name "Bascanka" comes from the [Bašćanska ploča](https://en.wikipedia.org/wiki/Ba%C5%A1%C4%87anska_plo%C4%8Da) (Baska tablet) - a stone tablet from around 1100 AD, found in the Church of St. Lucy near Baska on the island of Krk, Croatia. It is one of the oldest known inscriptions in the Croatian language, written in Glagolitic script. The tablet documents a royal land donation by King Zvonimir and is a cornerstone of Croatian cultural heritage and literacy.

## Author

Josip Habjan (habjan@gmail.com)

## License

GNU General Public License Version 3
