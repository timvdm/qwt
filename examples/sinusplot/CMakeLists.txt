set(sinusplot_SRCS
  sinusplot.cpp
)

add_executable(sinusplot ${sinusplot_SRCS})
target_link_libraries(sinusplot qwt)
