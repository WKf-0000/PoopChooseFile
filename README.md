# PoopChooseFile

A header-only, pure C++ interactive terminal file picker. No curses, no third-party libraries. Just ANSI escape codes and `<filesystem>`.

> [!WARNING]
> **The content here is extremely similar to poop.** 💩

## Features
- **Header-only**: Just `#include` and go.💩
- **Zero Dependencies**: Only C++17 Standard Library.💩
- **Smooth Scrolling**: Custom viewport logic for large folders.💩
- **Cross-Platform**: Works on Windows (`conio.h`) and Unix (`termios.h`).💩
- **ANSI UI**: Hidden cursor, reverse-video highlighting, clean exit.💩

## Usage

```cpp
#include <iostream>
#include "poopchoosefile.hpp"

int main() {
    poop::init(); // Init terminal colors & UTF-8
    std::string file = poop::chooseFile(15); // 15 = max lines shown
    
    if (!file.empty()) {
        std::cout << "Selected: " << file << "\n";
    }
    return 0;
}
```

## Controls
- **Up/Down Arrows**: Move cursor
- **Enter**: Open folder / Select file
- **ESC**: Cancel and exit

## License
[MIT](https://choosealicense.com/licenses/mit/)

-------

*Made with 💩.*

