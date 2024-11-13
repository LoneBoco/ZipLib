find_package(BZip2)
find_package(LibLZMA)
find_package(ZLIB)

if(NOT BZip2_DIR AND NOT BZIP2_INCLUDE_DIR)
    add_subdirectory(bzip2)
endif()

if(NOT LibLZMA_DIR AND NOT LibLZMA_INCLUDE_DIR)
    add_subdirectory(lzma)
endif()

if(NOT ZLIB_DIR AND NOT ZLIB_INCLUDE_DIR)
    add_subdirectory(zlib)
endif()
