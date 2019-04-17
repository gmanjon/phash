cmake_minimum_required(VERSION 3.13)
project(pHash_0_9_6)

set(CMAKE_CXX_STANDARD 14)

include_directories(/home/gmanjon/.sdkman/candidates/java/current/include)
include_directories(/home/gmanjon/.sdkman/candidates/java/current/include/linux)
include_directories(.)
include_directories(bindings/java)
include_directories(src)

add_executable(pHash_0_9_6
        bindings/java/pHash-jni.cpp
        bindings/java/pHash-jni.h
        bindings/java/pHash_MVPTree.h
        examples/test_audiophash.cpp
        examples/test_dctvideohash.cpp
        examples/test_imagephash.cpp
        examples/test_mhimagehash.cpp
        examples/test_texthash.cpp
        examples/test_texthash2.cpp
        src/audiophash.cpp
        src/audiophash.h
        src/cimgffmpeg.cpp
        src/cimgffmpeg.h
        src/ph_fft.c
        src/ph_fft.h
        src/pHash.cpp
        src/pHash.h
        config.h
        pHash-config.h)
