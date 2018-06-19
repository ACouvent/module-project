ADD_EXECUTABLE(demo demo.cpp)

ADD_LIBRARY(student STATIC student.cpp)

TARGET_LINK_LIBRARIES(demo student)
