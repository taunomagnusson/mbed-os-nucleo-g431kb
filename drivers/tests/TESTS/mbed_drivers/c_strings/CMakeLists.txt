# Copyright (c) 2020 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

cmake_minimum_required(VERSION 3.19.0 FATAL_ERROR)

set(MBED_PATH ${CMAKE_CURRENT_SOURCE_DIR}/../../../../.. CACHE INTERNAL "")
set(TEST_TARGET mbed-drivers-c-strings)

include(${MBED_PATH}/tools/cmake/mbed_greentea.cmake)

project(${TEST_TARGET})

mbed_greentea_cmake_macro(TEST_NAME ${TEST_TARGET})
