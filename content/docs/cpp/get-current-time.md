---
title: Get Current Time C++
type: docs
---

# `C++` : Get current time

# C++ 11
```c++
#include <iostream>
#include <chrono>
#include <ctime>    

int main()
{
    auto now = std::chrono::system_clock::now();
}
```
