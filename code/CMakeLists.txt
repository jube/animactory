include_directories("${CMAKE_CURRENT_SOURCE_DIR}/include")


add_library(animactory0
  lib/Factory.cc
)
qt5_use_modules(animactory0 Core Gui)


add_executable(animactory bin/animactory.cc)
target_link_libraries(animactory
  animactory0
)


install(
  DIRECTORY "${CMAKE_SOURCE_DIR}/include/animactory"
  DESTINATION "${CMAKE_INSTALL_INCLUDEDIR}"
)
