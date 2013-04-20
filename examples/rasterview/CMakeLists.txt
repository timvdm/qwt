set(rasterview_HDRS
  plot.h
)

set(rasterview_SRCS
  main.cpp
  plot.cpp
)

qt4_wrap_cpp(rasterview_MOC_HDRS ${rasterview_HDRS})

add_executable(rasterview ${rasterview_MOC_HDRS} ${rasterview_SRCS})
target_link_libraries(rasterview qwt)
