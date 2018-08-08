# Copyright (C) 2018  CERN for the benefit of the LHCb collaboration
# Author: Paul Seyfert <pseyfert@cern.ch>
#
# This software is distributed under the terms of the GNU General Public
# Licence version 3 (GPL Version 3), copied verbatim in the file "LICENSE".

# In applying this licence, CERN does not waive the privileges and immunities
# granted to it by virtue of its status as an Intergovernmental Organization
# or submit itself to any jurisdiction.

cmake_minimum_required(VERSION 3.11.4)
project(masked_user_range VERSION 0.0)

find_package(masked_range REQUIRED)

add_executable(masked_int masked_int.cpp)
target_link_libraries(masked_int
  PUBLIC
  masked_range
  )

