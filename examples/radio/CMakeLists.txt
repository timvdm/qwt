set(radio_HDRS
  ampfrm.h
  tunerfrm.h
)

set(radio_SRCS
  ampfrm.cpp
  mainwindow.cpp
  radio.cpp
  tunerfrm.cpp
)

qt4_wrap_cpp(radio_MOC_HDRS ${radio_HDRS})

add_executable(radio ${radio_MOC_HDRS} ${radio_SRCS})
target_link_libraries(radio qwt)
