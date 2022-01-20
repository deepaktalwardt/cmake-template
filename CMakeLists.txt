cmake_minimum_required(VERSION 3.6)
set(CMAKE_CXX_STANDARD 17)
project(cmake-template)

if(CMAKE_COMPILER_IS_GNUCXX OR CMAKE_CXX_COMPILER_ID MATCHES "Clang")
  add_compile_options(-Wall -Wextra -Wpedantic)
endif()

# Include headers
include_directories(
    include
)

## Libraries
# add_library(${PROJECT_NAME}
#   src/lib1
# )

# Executables
add_executable(main
    src/main.cpp
)

# target_link_libraries(main
#     ${PROJECT_NAME}
# )
