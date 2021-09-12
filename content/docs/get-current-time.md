---
title: Get Current Time
type: docs
bookToC: false
---

# How to get current time in...

{{< tabs "uniqueid" >}}
{{< tab "C++" >}}

## C++ 11

```c++
#include <iostream>
#include <chrono>   

int main()
{

    auto now = std::chrono::system_clock::now();
    std::time_t now_time = std::chrono::system_clock::to_time_t(now);
    std::cout<<std::ctime(&now_time);

    return 0;
}                                  
```

[Run this example](https://onlinegdb.com/2d8mOd9hg)

## C++ 03 and earlier

```c++
#include <iostream>
#include <ctime>

int main()
{
    std::time_t t = std::time(0);
    std::tm* now = std::localtime(&t);
    std::cout << std::asctime(now);

    return 0;
}
```

[Run this example](https://onlinegdb.com/3WJ0vVAFu)

{{< /tab >}}

{{< tab "Python" >}}

## As `datetime`

```python
from datetime import datetime

now = datetime.now()
print(now)
```
[Run this example](https://onlinegdb.com/whxX8OlLr)

## As epoch in Seconds

```python
import time
now = round(time.time())
print(now)
```
[Run this example](https://onlinegdb.com/JFh0BYeJq)

{{< /tab >}}

{{< tab "Java" >}}

## Using `LocalDatetime`

```java
import java.time.LocalDateTime;

public class Main
{
	public static void main(String[] args) {
		LocalDateTime now = LocalDateTime.now();
        System.out.println(now);
	}
}
```

[Run this example](https://onlinegdb.com/VRTpQ_xs7)
{{< /tab >}}
{{< /tabs >}}