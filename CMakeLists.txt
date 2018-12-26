cmake_minimum_required(VERSION 3.4)

project(screensaver)

    find_package(X11 REQUIRED)
    find_package(OpenGL REQUIRED)

    add_executable(${PROJECT_NAME} src/main.cpp)
    target_link_libraries(${PROJECT_NAME} X11 ${OPENGL_LIBRARIES})
