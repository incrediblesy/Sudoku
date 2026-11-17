# Sudoku Game in Flutter

A fully-featured Sudoku game built with **Flutter** and **Flutter Bloc**. Play Sudoku with multiple difficulty levels, notes, undo/redo, timers, and error/mistake tracking. Supports **dark mode** and highlights conflicts dynamically.

## Platform Support

| Platform | Supported |
| -------- | --------- |
| Android  | Yes ✅    |
| iOS      | Yes ✅    |
| Web      | Yes ✅    |
| macOS    | Yes ✅    |
| Linux    | Yes ✅    |
| Windows  | Yes ✅    |

## Features

-   **Classic Sudoku Gameplay**  
    9x9 Sudoku grid with selectable cells.

-   **Difficulty Levels**

    -   Easy
    -   Medium
    -   Hard
    -   Expert

-   **Notes Mode**  
    Add small notes to cells for potential numbers.

-   **Undo & Redo**  
    Revert or reapply your moves.

-   **Timer**  
    Track the time elapsed while playing.

-   **Mistake Tracking**  
    Set a maximum number of mistakes (default: 3). The game ends if you exceed this limit.

-   **Win / Lose Detection**  
    Automatically detects when the puzzle is completed or when maximum mistakes are reached.

-   **Conflict Highlighting**  
    Highlights conflicts in the current row, column, and 3x3 box.

-   **Dark Mode Support**  
    Adapts to the system theme automatically.

## Screenshots

[light]: assets/screenshots/light.png
[dark]: assets/screenshots/dark.png

|   Light Mode    |   Dark Mode   |
| :-------------: | :-----------: |
| ![Light][light] | ![Dark][dark] |

## Getting Started

### Prerequisites

-   Flutter SDK >= 3.0
-   Dart >= 3.0
-   IDE: VS Code, Android Studio, or any Flutter-compatible IDE

### Installation

1. Clone the repository:

```bash
git clone https://github.com/shokhrukhbekyuldoshev/sudoku.git
cd sudoku
```

1. Install dependencies:

```bash
flutter pub get
```

3. Run the app:

```bash
flutter run
```

## Project Structure

```
lib/
├─ core/               # Core classes(theme, helpers, constants)
├─ data/
│  ├─ models/           # Difficulty models
│  └─ repositories/     # Storage for game state
├─ logic/
│  ├─ cubit/            # GameCubit and GameState
│  └─ services/         # Sudoku puzzle generator
├─ ui/
│  ├─ widgets/          # SudokuBoard and other UI widgets
│  └─ screens/          # GameScreen and other UI screens
├─ utils/               # Utility functions
└─ main.dart
```

## Usage

-   Tap a cell to select it.
-   Enter numbers to fill the grid.
-   Use **notes mode** to add hints to a cell.
-   Undo or redo moves using the respective buttons.
-   The timer starts automatically when the puzzle loads.
-   Mistakes are tracked, and the game ends if you reach the maximum allowed mistakes.
-   Conflicts are highlighted dynamically.

## Dependencies

| Name                                                                      | Version | Description                                                    |
| ------------------------------------------------------------------------- | ------- | -------------------------------------------------------------- |
| [bloc](https://pub.dev/packages/bloc)                                     | ^9.0.0  | A predictable state management library                         |
| [equatable](https://pub.dev/packages/equatable)                           | ^2.0.7  | An equatable package for Flutter                               |
| [flutter_bloc](https://pub.dev/packages/flutter_bloc)                     | ^9.1.1  | A package for easily implementing BLoC architecture in Flutter |
| [flutter_launcher_icons](https://pub.dev/packages/flutter_launcher_icons) | ^0.14.4 | A package for adding launcher icons to Flutter apps            |
| [shared_preferences](https://pub.dev/packages/shared_preferences)         | ^2.5.3  | A Flutter package for accessing the shared preferences.        |

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

Distributed under the Attribution-NonCommercial-ShareAlike 4.0 International License. See [LICENSE](LICENSE) for more information.

## Contact

-   [Email](mailto:shokh.xyz@gmail.com)
-   [GitHub](https://github.com/incrediblesy)

## Show your support

Give a ⭐️ if you like this project!
