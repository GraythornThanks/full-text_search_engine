file(GLOB_RECURSE srcs CONFIGURE_DEPENDS src/*.cpp include/*.h)
add_executable(testEchoServer ${srcs})

target_include_directories(testEchoServer PUBLIC include)

target_link_libraries(testEchoServer PUBLIC reactor)
