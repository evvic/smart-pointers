# smart-pointers
Implementation of C++ memory.h library

### Build GTest program
``` bash
# Project root
cmake .
make
```
- This will build a `Makefile` based on CMakeLists.txt
- Then run the makefile to compile the .cpp gtest code



### Setup GTest
- Add GTest as a submodule
``` bash
git submodule add https://github.com/google/googletest.git googletest

```

### Manually Running GTest

Build
``` bash
cd googletest
mkdir build
cd build
cmake .. -DBUILD_GMOCK=OFF
make
cd ../..
g++ example.cpp googletest/build/lib/libgtest.a googletest/build/lib/libgtest_main.a -lpthread -I googletest/googletest/include/
```

Run
``` bash
# In repo root
./a.out
```

