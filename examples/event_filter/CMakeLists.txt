set(event_filter_HDRS
  canvaspicker.h
  colorbar.h
  plot.h
  scalepicker.h
)

set(event_filter_SRCS
  canvaspicker.cpp
  colorbar.cpp
  event_filter.cpp
  plot.cpp
  scalepicker.cpp
)

qt4_wrap_cpp(event_filter_MOC_HDRS ${event_filter_HDRS})

add_executable(event_filter ${event_filter_MOC_HDRS} ${event_filter_SRCS})
target_link_libraries(event_filter qwt)
