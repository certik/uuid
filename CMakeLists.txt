cmake_minimum_required(VERSION 2.6)

project(uuid)

set(LIBUUID_VERSION 2.15.1)

add_subdirectory(src)

configure_file (
    ${uuid_SOURCE_DIR}/uuid.pc.in
    ${uuid_BINARY_DIR}/libuuid.pc
@ONLY)

install (
    FILES ${uuid_BINARY_DIR}/libuuid.pc
    DESTINATION lib/pkgconfig
)
