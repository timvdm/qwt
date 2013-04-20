set(dials_HDRS
  attitude_indicator.h
  cockpit_grid.h
)

set(dials_SRCS
  attitude_indicator.cpp
  cockpit_grid.cpp
  compass_grid.cpp
  dials.cpp
  speedo_meter.cpp
)

qt4_wrap_cpp(dials_MOC_HDRS ${dials_HDRS})

add_executable(dials ${dials_MOC_HDRS} ${dials_SRCS})
target_link_libraries(dials qwt)
