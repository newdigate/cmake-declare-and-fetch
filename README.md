# cmake-declare-and-fetch
cmake git build macro
* copy `cmake_declare_and_fetch.cmake.in` to your local project root directory.
* add to your CMakeLists.txt
  ```cmake
  include(cmake_declare_and_fetch.cmake.in)
  DeclareAndFetch(teensy_x86_stubs                https://github.com/newdigate/teensy-x86-stubs.git main src)
  ```
