[README_2.md](https://github.com/user-attachments/files/28198026/README_2.md)
# 3DAGame 🎮

> My first ever video game — built with Unity 2021 for the Universal Windows Platform (UWP).

---

## About

A 3D game built in Unity 2021 and exported as a Universal Windows Platform (UWP) application. The game logic is written in C# and compiled to native C++ via Unity's IL2CPP scripting backend.

---

## Requirements

- **Windows 10 or 11**
- **Visual Studio** (any recent version) — download from https://visualstudio.microsoft.com/

During installation, select the **Universal Windows Platform development** workload, and make sure **C++ Universal Windows Platform tools** is checked inside it (it's unchecked by default).

> ⚠️ You do **not** need Unity. The repo already contains the fully generated C++ output — just open and compile in Visual Studio.

---

## Building & Running

1. Clone the repository:
   ```bash
   git clone https://github.com/YounessX3/3DAGame.git
   cd 3DAGame
   ```

2. Open `3Dahhgame.sln` in Visual Studio.

3. Select a configuration and platform (e.g. `Release | x64`).

4. Build the solution (`Ctrl+Shift+B`).

5. Deploy to **Local Machine** or press `F5` to build and run.

> ⚠️ Make sure **Developer Mode** is enabled: `Settings → Update & Security → For developers → Developer Mode`

---

## Project Structure

```
3DAGame/
├── 3Dahhgame/                              # Main UWP app project
├── Il2CppOutputProject/                    # IL2CPP-generated C++ code
├── 3Dahhgame_BurstDebugInformation_DoNotShip/
├── 3Dahhgame.sln                           # Visual Studio solution
└── UnityCommon.props                       # Shared MSBuild properties
```

---

## Tech Stack

- **Engine:** Unity 2021 (export only)
- **Platform:** Universal Windows Platform (UWP)
- **Scripting backend:** IL2CPP (C# → C++)
- **IDE:** Visual Studio
- **Architectures:** x86, x64, ARM, ARM64
