set(spectrogram_HDRS
  plot.h
)

set(spectrogram_SRCS
  main.cpp
  plot.cpp
)

qt4_wrap_cpp(spectrogram_MOC_HDRS ${spectrogram_HDRS})

add_executable(spectrogram ${spectrogram_MOC_HDRS} ${spectrogram_SRCS})
target_link_libraries(spectrogram qwt)
