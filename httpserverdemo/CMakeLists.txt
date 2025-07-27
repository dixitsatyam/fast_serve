project(demo)

set(CMAKE_CXX_STANDARD 17)

#http server build

add_executable(httpserverdemo httpserverdemo.cpp)
target_link_libraries(httpserverdemo httpserver)
set(INCLUDE_SERVER_DIRS "../httpserver")
# target_include_directories(server PUBLIC ${INCLUDE_SERVER_DIRS})