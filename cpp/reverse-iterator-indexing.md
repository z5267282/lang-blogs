To access the position of a reverse iterator, you still subtract it from `rbegin`.

```cpp
#include <algorithm>
#include <cassert>
#include <iostream>

int main() {
    auto vec = std::vector<int>{1 , 3 , 5 , 10, 14, 18};
    //                                          j
    // reverse indices
    //                          5   4   3   2   1   0
    auto j = ++vec.rbegin();
    assert(*j == 14);
    auto j_idx = j - vec.rbegin();
    assert (j_idx == 1);
}
```