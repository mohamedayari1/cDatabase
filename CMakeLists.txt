cmake_minimum_required(VERSION 3.10)

# 1. Project Name
project(cDatabase LANGUAGES C)

# 2. Compilation Settings
set(CMAKE_C_STANDARD 17)
set(CMAKE_C_STANDARD_REQUIRED ON)

# 3. Include Headers
# This tells the compiler to look in the /include folder for .h files
include_directories(include)

# 4. Define Source Files
# List all your .c files here as you create them
set(SOURCES 
    src/main.c
    # src/database.c  <-- Add your new files here
    # src/utils.c
)

# 5. Create Executable
# We use the variable ${SOURCES} to keep the command clean
add_executable(app ${SOURCES})