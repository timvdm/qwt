set(plotmatrix_HDRS
  plotmatrix.h
)

set(plotmatrix_SRCS
  main.cpp
  plotmatrix.cpp
)

qt4_wrap_cpp(plotmatrix_MOC_HDRS ${plotmatrix_HDRS})

add_executable(plotmatrix ${plotmatrix_MOC_HDRS} ${plotmatrix_SRCS})
target_link_libraries(plotmatrix qwt)
