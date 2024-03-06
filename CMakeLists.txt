set(CMAKE_SYSTEM_NAME Generic)
set(CMAKE_SYSTEM_PROCESSOR aarch64)

set(CMAKE_TRY_COMPILE_TARGET_TYPE STATIC_LIBRARY)

set(COMPILER_PREFIX "aarch64-none-elf")

set(CMAKE_C_COMPILER ${COMPILER_PREFIX}-gcc)
set(CMAKE_CXX_COMPILER ${COMPILER_PREFIX}-g++)
set(CMAKE_LINKER ${COMPILER_PREFIX}-ld)



add_executable(hello_world.elf)

# Add the source files to the target
target_sources(hello_world.elf PRIVATE
    startup.s
    hello_world.c
)

# Add compiler flags, if needed
# target_compile_options(hello_world.elf PRIVATE <flags>)

# Add linker flags, if needed
# target_link_options(hello_world.elf PRIVATE <flags>)