add_executable(custom_frame_window WIN32)

target_sources(custom_frame_window PRIVATE main.cpp)

# TODO: Add /WX
target_compile_options(custom_frame_window PRIVATE /Wall)

target_compile_definitions(custom_frame_window PRIVATE UNICODE _UNICODE)

target_include_directories(custom_frame_window PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})

target_link_libraries(custom_frame_window PRIVATE uxtheme.lib)
