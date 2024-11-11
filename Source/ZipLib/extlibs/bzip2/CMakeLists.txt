# source files
set(sources
    blocksort.c
    bzerror.c
    bzlib_private.h
    bzlib.c
    bzlib.h
    compress.c
    crctable.c
    decompress.c
    huffman.c
    randtable.c
)
# library
add_library(bzip2 STATIC
    ${sources}
)
add_library(BZip2::BZip2 ALIAS bzip2)
add_library(bz2_static ALIAS bzip2)

#properties
target_include_directories(bzip2
    PUBLIC
        .
)
set_target_properties(bzip2
    PROPERTIES
        FOLDER "External libraries"
)
