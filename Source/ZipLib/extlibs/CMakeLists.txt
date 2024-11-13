find_package(BZip2)
find_package(LibLZMA CONFIG)
find_package(ZLIB)

if(NOT BZip2_FOUND)
    add_subdirectory(bzip2)
endif()

if(NOT LibLZMA_FOUND)
    add_subdirectory(lzma)
endif()

if(NOT ZLIB_FOUND)
    add_subdirectory(zlib)
endif()
