cmake_minimum_required(VERSION 3.16)
project(ipvsadm_1_26 C)

set(CMAKE_C_STANDARD 11)

include_directories(.)
include_directories(libipvs)

add_executable(ipvsadm_1_26
        libipvs/ip_vs.h
        libipvs/ip_vs_nl_policy.c
        libipvs/libipvs.c
        libipvs/libipvs.h
        config_stream.c
        config_stream.h
        dynamic_array.c
        dynamic_array.h
        ipvsadm.c)
