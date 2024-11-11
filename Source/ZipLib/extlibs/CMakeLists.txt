if(NOT BZIP2_FOUND)
    add_subdirectory(bzip2)
endif()

if(NOT LIBLZMA_FOUND)
    add_subdirectory(lzma)
endif()

if(NOT ZLIB_FOUND)
    add_subdirectory(zlib)
endif()
