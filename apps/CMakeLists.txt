add_executable(sam main.c)

if(USESDL)
  find_package(SDL REQUIRED)
  add_compile_definitions(USESDL)
endif()

target_include_directories(sam PRIVATE ${SDL_INCLUDE_DIR})
target_link_libraries(sam PRIVATE libsam ${SDL_LIBRARY})
