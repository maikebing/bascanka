# Bascanka

An open-source text editor for Windows built with .NET and WinForms, with zero third-party dependencies. Named after the [Bascanska ploca](https://en.wikipedia.org/wiki/Ba%C5%A1%C4%87anska_plo%C4%8Da), one of the oldest known inscriptions in the Croatian language.

## Features

- Syntax highlighting for common languages (C#, JavaScript, Python, HTML, CSS, JSON, XML, and more)
- Code folding
- Find & replace with regex support
- Hex editor
- Macro recording and playback
- Tab-based editing
- Word wrap
- Plugin system
- Multilanguage UI (English and Croatian built-in, extensible via JSON)
- Theming support

## Requirements

- Windows 10 or later
- [.NET 10 Runtime](https://dotnet.microsoft.com/download)

## Build

```
dotnet build src/Bascanka.App/Bascanka.App.csproj
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

The name "Bascanka" comes from the Bascanska ploca (Baska tablet) - a stone tablet from around 1100 AD, found in the Church of St. Lucy near Baska on the island of Krk, Croatia. It is one of the oldest known inscriptions in the Croatian language, written in Glagolitic script. The tablet documents a royal land donation by King Zvonimir and is a cornerstone of Croatian cultural heritage and literacy.

## Author

Josip Habjan (habjan@gmail.com)

## License

GNU GENERAL PUBLIC LICENSE Version 3
