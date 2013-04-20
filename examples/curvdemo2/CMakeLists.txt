set(curvdemo2_SRCS
  curvdemo2.cpp
)

add_executable(curvdemo2 ${curvdemo2_SRCS})
target_link_libraries(curvdemo2 qwt)
