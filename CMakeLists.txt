cmake_minimum_required(VERSION 3.5)

project(dftd3)
enable_language(Fortran)

if(CMAKE_Fortran_COMPILER_ID MATCHES "Intel")
    set(dialect "-stand f90")
endif()

set(CMAKE_Fortran_FLAGS "${CMAKE_Fortran_FLAGS} ${dialect}")

add_executable(dftd3 dftd3.f copyc6.f)

install(TARGETS dftd3 RUNTIME DESTINATION "bin")
