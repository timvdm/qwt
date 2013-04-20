set(curvdemo1_SRCS
  curvdemo1.cpp
)

add_executable(curvdemo1 ${curvdemo1_SRCS})
target_link_libraries(curvdemo1 qwt)
