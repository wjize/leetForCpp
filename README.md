# leetForCpp

## CMakeLists.txt
由于每次添加文件，cmakelists都要变化，合并时会冲突。所以在此单独记录
```c++
cmake_minimum_required(VERSION 3.25)
project(leetForCpp)

set(CMAKE_CXX_STANDARD 11)

#boost库
set(BOOST_ROOT "/opt/homebrew/Cellar/boost/1.81.0_1/include/boost")
include_directories(/opt/homebrew/Cellar/boost/1.81.0_1/include)
link_directories(/opt/homebrew/Cellar/boost/1.81.0_1/lib)

#pcre++库
set(PCRE "/opt/homebrew/Cellar/pcre/8.45/include/*")
include_directories(/opt/homebrew/Cellar/pcre/8.45/include)
link_directories(/opt/homebrew/Cellar/pcre/8.45/lib)

add_executable(leetForCpp main.cpp)
```