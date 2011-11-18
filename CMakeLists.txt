# Copyright (C) 2007-2011 LuaDist.
# Submited by Peter Kapec
# Redistribution and use of this file is allowed according to the terms of the MIT license.
# For details see the COPYRIGHT file distributed with LuaDist.
# Please note that the package source code is licensed under its own license.

PROJECT(ldoc NONE)
CMAKE_MINIMUM_REQUIRED(VERSION 2.6)
INCLUDE(dist.cmake)

install_lua_executable ( ldoc ldoc.lua )
INSTALL(DIRECTORY ldoc DESTINATION ${INSTALL_LMOD})

INSTALL(FILES readme.md COPYRIGHT DESTINATION ${INSTALL_DATA})
INSTALL(DIRECTORY docs/ DESTINATION ${INSTALL_DOC})
INSTALL(DIRECTORY tests/ DESTINATION ${INSTALL_TEST})


