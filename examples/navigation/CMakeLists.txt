set(navigation_HDRS
  mainwindow.h
  plot.h
)

set(navigation_SRCS
  main.cpp
  mainwindow.cpp
  plot.cpp
)

qt4_wrap_cpp(navigation_MOC_HDRS ${navigation_HDRS})

add_executable(navigation ${navigation_MOC_HDRS} ${navigation_SRCS})
target_link_libraries(navigation qwt)
