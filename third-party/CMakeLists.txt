# Bundle RKH framework and Blinky application
if (EXISTS ${CMAKE_CURRENT_SOURCE_DIR}/RKH)
    # Custom module and scripts
    include(${CMAKE_CURRENT_SOURCE_DIR}/RKH/cmake/boilerplate.cmake)
    add_subdirectory(RKH)
else()
    message(FATAL_ERROR "RKH do not found in ${CMAKE_CURRENT_SOURCE_DIR}")
endif()
