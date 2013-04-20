set(sysinfo_SRCS
  sysinfo.cpp
)

add_executable(sysinfo ${sysinfo_SRCS})
target_link_libraries(sysinfo qwt)
