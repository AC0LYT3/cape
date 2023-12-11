# CMakeList.txt : CMake project for cape, include source and define
# project specific logic here.
#

# Set CXXFLAGS
include_directories (include)

# Add source to this project's executable.
add_executable (cape "src/cape.cpp" "include/cape.h")

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET cape PROPERTY CXX_STANDARD 20)
endif()

# TODO: Add tests and install targets if needed.
