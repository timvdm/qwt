set(svgmap_HDRS
  plot.h
)

set(svgmap_SRCS
  main.cpp
  plot.cpp
)

qt4_wrap_cpp(svgmap_MOC_HDRS ${svgmap_HDRS})

add_executable(svgmap ${svgmap_MOC_HDRS} ${svgmap_SRCS})
target_link_libraries(svgmap qwt)
