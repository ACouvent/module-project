ADD_EXECUTABLE(demo demo.cpp)
ADD_EXECUTABLE(test1 test1.cpp)
ADD_EXECUTABLE(test2 test2.cpp)

ADD_LIBRARY(student STATIC student.cpp)

TARGET_LINK_LIBRARIES(demo student)
TARGET_LINK_LIBRARIES(test1 student)
TARGET_LINK_LIBRARIES(test2 student)

ENABLE_TESTING()
ADD_TEST( test1 demo )
ADD_TEST( test2 demo )


