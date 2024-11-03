# Hello World

&ensp;以下是一个 C++ Hello World 程序。
```cpp
// main.cpp
#include <iostream>

int main() {
    std::cout << "Hello, World!" << std::endl;
    return 0;
}
```

## note 01 `std::endl` 与 `\n` 的异同
- 同: 两者均将新行插入到流中。
- 异: 
  - `std::endl` 会将当前缓冲区中的所有内容输出到通道中。如果过度使用 `std::endl`（特别是在循环里使用 `std::endl`），会影响程序性能。
  - `\n` 不会自动刷新缓冲区。
