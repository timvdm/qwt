set(friedberg_HDRS
  plot.h
)

set(friedberg_SRCS
  friedberg2007.cpp
  main.cpp
  plot.cpp
)

qt4_wrap_cpp(friedberg_MOC_HDRS ${friedberg_HDRS})

add_executable(friedberg ${friedberg_MOC_HDRS} ${friedberg_SRCS})
target_link_libraries(friedberg qwt)
