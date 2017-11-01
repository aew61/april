cmake_minimum_required(VERSION 3.0)

project(parser C)

get_filename_component(SRC_DIR ${BASE_SRC_ROOT}/parser ABSOLUTE)
get_filename_component(INC_DIR ${BASE_INC_ROOT}/april/parser ABSOLUTE)

set(${PROJECT_NAME}_SRCS
    ${SRC_DIR}/parser.c
)

set(${PROJECT_NAME}_PRIV_HDRS

)

set(${PROJECT_NAME}_PUB_HDRS
    ${INC_DIR}/parser.h
)

add_library(${PROJECT_NAME} SHARED
    ${${PROJECT_NAME}_SRCS} ${${PROJECT_NAME}_PRIV_HDRS} ${${PROJECT_NAME}_PUB_HDRS}
)

