set(bode_HDRS
  mainwindow.h
  plot.h
)

set(bode_SRCS
  main.cpp
  mainwindow.cpp
  plot.cpp
)

qt4_wrap_cpp(bode_MOC_HDRS ${bode_HDRS})

add_executable(bode ${bode_MOC_HDRS} ${bode_SRCS})
target_link_libraries(bode qwt)
