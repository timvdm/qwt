set(cpuplot_HDRS
  cpuplot.h
)

set(cpuplot_SRCS
  cpupiemarker.cpp
  cpuplot.cpp
  cpustat.cpp
)

qt4_wrap_cpp(cpuplot_MOC_HDRS ${cpuplot_HDRS})

add_executable(cpuplot ${cpuplot_MOC_HDRS} ${cpuplot_SRCS})
target_link_libraries(cpuplot qwt)
