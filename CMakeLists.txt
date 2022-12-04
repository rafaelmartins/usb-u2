# SPDX-FileCopyrightText: 2021-2022 Rafael G. Martins <rafael@rafaelmartins.eng.br>
# SPDX-License-Identifier: BSD-3-Clause

cmake_minimum_required(VERSION 3.19)

project(usb-u2 C)

add_library(usb-u2 INTERFACE)

target_sources(usb-u2 INTERFACE
    usb-u2.c
    usb-u2.h
)

target_include_directories(usb-u2 INTERFACE
    ${CMAKE_CURRENT_LIST_DIR}
)
