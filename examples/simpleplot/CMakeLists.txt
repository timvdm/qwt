set(simpleplot_SRCS
  simpleplot.cpp
)

add_executable(simpleplot ${simpleplot_SRCS})
target_link_libraries(simpleplot qwt)
