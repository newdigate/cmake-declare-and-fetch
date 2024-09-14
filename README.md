# cmake-declare-and-fetch
cmake git build macro

```cmake
#********** CMAKE DECLARE AND FETCH MACRO ******
include(FetchContent)
FetchContent_Declare(cmake_declare_and_fetch
        GIT_REPOSITORY https://github.com/newdigate/cmake-declare-and-fetch.git
        GIT_TAG        main
)
FetchContent_MakeAvailable(cmake_declare_and_fetch)
include("${FETCHCONTENT_BASE_DIR}/cmake_declare_and_fetch-src/DeclareAndFetchCMake.in")
#********** CMAKE DECLARE AND FETCH MACRO ******
```