# Copyright (c) 2022 Konstantin Selin
# Copyright (c) 2018 Nordic Semiconductor
#
# SPDX-License-Identifier: MIT-Modern-Variant
#
cmake_minimum_required(VERSION 3.20.0)

find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})
project(NONE)

# NORDIC SDK APP START
target_sources(app PRIVATE
  src/main.c
)

target_include_directories(app PRIVATE .)
# NORDIC SDK APP END
