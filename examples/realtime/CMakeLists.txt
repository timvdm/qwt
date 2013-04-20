set(realtime_HDRS
  incrementalplot.h
  mainwindow.h
  randomplot.h
  scrollbar.h
  scrollzoomer.h
)

set(realtime_SRCS
  incrementalplot.cpp
  main.cpp
  mainwindow.cpp
  randomplot.cpp
  scrollbar.cpp
  scrollzoomer.cpp
)

qt4_wrap_cpp(realtime_MOC_HDRS ${realtime_HDRS})

add_executable(realtime ${realtime_MOC_HDRS} ${realtime_SRCS})
target_link_libraries(realtime qwt)

