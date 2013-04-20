include_directories(../src)

set(qwt_mathml_SRCS
  mathml/qwt_mathml_text_engine.cpp
  mathml/qwt_mml_document.cpp
)

add_library(qwt_mathml SHARED ${qwt_mathml_SRCS})
target_link_libraries(qwt_mathml qwt)
