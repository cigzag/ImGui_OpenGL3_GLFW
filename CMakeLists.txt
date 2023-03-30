cmake_minimum_required(VERSION 3.24)
project (ImGui_Test)

set(CMAKE_CXX_STANDARD 23)

find_package(glfw3 REQUIRED)
find_package(OpenGL REQUIRED)

add_executable(ImGui_Test src/main.cpp src/imgui/imgui.cpp src/imgui/imgui_draw.cpp src/imgui/imgui_tables.cpp src/imgui/imgui_widgets.cpp src/imgui/backends/imgui_impl_glfw.cpp src/imgui/backends/imgui_impl_opengl3.cpp src/imgui/imgui_demo.cpp)

target_link_libraries(ImGui_Test glfw OpenGL)