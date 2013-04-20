set(tvplot_HDRS
  tvplot.h
)

set(tvplot_SRCS
  main.cpp
  tvplot.cpp
)

qt4_wrap_cpp(tvplot_MOC_HDRS ${tvplot_HDRS})

add_executable(tvplot ${tvplot_MOC_HDRS} ${tvplot_SRCS})
target_link_libraries(tvplot qwt)
