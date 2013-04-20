set(refreshtest_HDRS
  panel.h
  plot.h
)

set(refreshtest_SRCS
  circularbuffer.cpp
  main.cpp
  mainwindow.cpp
  panel.cpp
  plot.cpp
)

qt4_wrap_cpp(refreshtest_MOC_HDRS ${refreshtest_HDRS})

add_executable(refreshtest ${refreshtest_MOC_HDRS} ${refreshtest_SRCS})
target_link_libraries(refreshtest qwt)

