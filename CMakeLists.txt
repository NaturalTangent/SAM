cmake_minimum_required(VERSION 3.13)

project(SAM VERSION 1.0
            DESCRIPTION "Software Automated Mouth"
            LANGUAGES C)

option(USESDL "Enable SDL support" ON)

# The compiled library code is here
add_subdirectory(src)

# The executable code is here
add_subdirectory(apps)

