set(oscilloscope_HDRS
  knob.h
  mainwindow.h
  plot.h
  samplingthread.h
  wheelbox.h
)

set(oscilloscope_SRCS
  curvedata.cpp
  knob.cpp
  main.cpp
  mainwindow.cpp
  plot.cpp
  samplingthread.cpp
  signaldata.cpp
  wheelbox.cpp
)

qt4_wrap_cpp(oscilloscope_MOC_HDRS ${oscilloscope_HDRS})

add_executable(oscilloscope ${oscilloscope_MOC_HDRS} ${oscilloscope_SRCS})
target_link_libraries(oscilloscope qwt)
