cmake_minimum_required(VERSION 3.10)
project(CourseManagementSystem)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Source files
set(SOURCES
    User.cpp
    Student.cpp
    Instructor.cpp
    DepartmentHead.cpp
    SystemAdmin.cpp
    Department.cpp
    Course.cpp
    Schedule.cpp
    Class.cpp
    main.cpp
)

# Header files
set(HEADERS
    User.h
    Student.h
    Instructor.h
    DepartmentHead.h
    SystemAdmin.h
    Department.h
    Course.h
    Schedule.h
    Class.h
)

# Create executable
add_executable(${PROJECT_NAME} ${SOURCES} ${HEADERS})

# Set output directory
set_target_properties(${PROJECT_NAME} PROPERTIES
    RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin
)


