# Computer Store Management System

A C++ console application for managing a small computer store's employee and inventory records. The project was built as an academic Object-Oriented Programming / Data Structures assignment and demonstrates class-based modeling, menu-driven workflows, file persistence, and CSV import/export.

## Features

- Head-manager login flow with a simple PIN gate
- Add and update employee records
- Add and update inventory items
- Search employee and inventory data
- Display all store records from the console
- Persist records to a binary file when the program exits
- Import and export records using CSV-style files

## Project Structure

```text
.
├── Computer Store.sln
├── Computer Store.vcxproj
├── Computer Store.vcxproj.filters
├── Main.cpp
├── items.csv
└── README.md
```

## Build

This project uses Microsoft Visual Studio C++ project files and calls MSVC-specific functions such as `strncpy_s`.

Open `Computer Store.sln` in Visual Studio 2022 and build the solution, or run from a Visual Studio Developer PowerShell:

```powershell
msbuild "Computer Store.sln" /p:Configuration=Release /p:Platform=x64
```

## Run

After building, run the executable from the build output directory:

```powershell
.\x64\Release\"Computer Store.exe"
```

The manager PIN shown by the program is:

```text
1111
```

Help mode:

```powershell
.\x64\Release\"Computer Store.exe" help
```

Export records:

```powershell
.\x64\Release\"Computer Store.exe" export items.csv
```

Import records:

```powershell
.\x64\Release\"Computer Store.exe" import items.csv
```

## Notes

- `Records.bin` is generated at runtime and is intentionally ignored by Git.
- `items.csv` is included as sample import/export data.
- Build outputs, Visual Studio cache files, archives, and local assignment documents are excluded from the repository.
