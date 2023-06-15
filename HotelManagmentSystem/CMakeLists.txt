# CMakeList.txt: projekt CMake dla elementu HotelManagmentSystem, dołącz źródło i zdefiniuj
# tutaj logikę specyficzną dla projektu.
#
cmake_minimum_required (VERSION 3.8)

# Enable Hot Reload for MSVC compilers if supported.
if (POLICY CMP0141)
  cmake_policy(SET CMP0141 NEW)
  set(CMAKE_MSVC_DEBUG_INFORMATION_FORMAT "$<IF:$<AND:$<C_COMPILER_ID:MSVC>,$<CXX_COMPILER_ID:MSVC>>,$<$<CONFIG:Debug,RelWithDebInfo>:EditAndContinue>,$<$<CONFIG:Debug,RelWithDebInfo>:ProgramDatabase>>")
endif()

project (HotelManagmentSystem)

# Dodaj źródło do pliku wykonywalnego tego projektu.
# add_executable (HotelManagmentSystem "HotelManagmentSystem.cpp" "HotelManagmentSystem.h")

add_subdirectory(program)
add_subdirectory(library)

# TODO: Dodaj testy i zainstaluj elementy docelowe w razie potrzeby.
