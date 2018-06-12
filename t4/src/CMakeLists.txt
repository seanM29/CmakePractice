INCLUDE_DIRECTORIES(/usr/include/hello)
ADD_EXECUTABLE(main main.c)
TARGET_LINK_LIBRARIES(main libhello.a)
