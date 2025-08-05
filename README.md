
# OBSBOT Interface


## For build in Fedora:

1. Beep
`sudo dnf install cmake gcc-c++ libstdc++-devel`

2.Boop
``` bash
mkdir -p build
cd build
cmake ../OBSBOT_Sample -DDEV_LIB_PATH=../linux/x86_64-release
make
```

MAYBE ADD `target_link_libraries(OBSBOT_Sample PRIVATE ${CMAKE_LIBRARY_PATH}/libdev.so)`

3. Beep
`LD_LIBRARY_PATH=../linux/x86_64-release ./OBSBOT_Sample <command>`

4. Boop
`alias obsbot='LD_LIBRARY_PATH=../linux/x86_64-release ./OBSBOT_Sample'`
