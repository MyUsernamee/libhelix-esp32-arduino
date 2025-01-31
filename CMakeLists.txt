
file(GLOB_RECURSE SRC_LIST_C "${PROJECT_SOURCE_DIR}/src/*.c" )

idf_component_register(SRCS ${SRC_LIST_C}
INCLUDE_DIRS "./src"
REQUIRES arduino-esp32)

set(CFLAGS -Wno-error)