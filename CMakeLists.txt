cmake_minimum_required(VERSION 2.6)
include($ENV{CHAOS_BUNDLE}/tools/project_template/CMakeChaos.txt)

SET(uicwrapper_example_exe_src UIToolkitCMDLineCWapperExample.c)

ADD_EXECUTABLE(ExampleUIToolkitCWrapper ${uicwrapper_example_exe_src})
TARGET_LINK_LIBRARIES(ExampleUIToolkitCWrapper chaos_uitoolkit chaos_common ${FrameworkLib} stdc++ m)

INSTALL_TARGETS(/bin ExampleUIToolkitCWrapper)