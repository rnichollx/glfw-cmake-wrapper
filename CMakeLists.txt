cmake_minimum_required(VERSION 3.15)

project(GLFWCMakeWrapper)

add_subdirectory(external/glfw)

install(TARGETS glfw EXPORT GLFWCMakeWrapper_exports)

export(EXPORT GLFWCMakeWrapper_exports NAMESPACE GLFWCMakeWrapper:: FILE GLFWCMakeWrapperConfig.cmake )
