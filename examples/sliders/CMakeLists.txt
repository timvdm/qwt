set(sliders_HDRS
  sliders.h
)

set(sliders_SRCS
  sliders.cpp
)

qt4_wrap_cpp(sliders_MOC_HDRS ${sliders_HDRS})

add_executable(sliders ${sliders_MOC_HDRS} ${sliders_SRCS})
target_link_libraries(sliders qwt)
