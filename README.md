# cmake-declare-and-fetch
cmake git build macro
```cmake
DeclareAndFetch(name git-url branch cmakeprefixes)
```
* cmakeprefixes is a semi-column delimited array of relative source paths to include
   
# usage
* copy `cmake_declare_and_fetch.cmake.in` to your local project root directory.
* add to your CMakeLists.txt
  ```cmake
    include(cmake_declare_and_fetch.cmake.in)
    DeclareAndFetch(teensy_x86_stubs https://github.com/newdigate/teensy-x86-stubs.git main src)
    DeclareAndFetch(teensy_x86_sd_stubs https://github.com/newdigate/teensy-x86-sd-stubs.git noinstall src)
    DeclareAndFetch(teensy_gfx https://github.com/newdigate/teensy-gfx.git noinstall src)
    DeclareAndFetch(teensy_x86_encoder_stubs https://github.com/newdigate/teensy-x86-encoder-stubs.git noinstall src)
    DeclareAndFetch(teensy_x86_bounce2_stubs https://github.com/newdigate/teensy-x86-bounce2-stubs.git noinstall src)
  ```
