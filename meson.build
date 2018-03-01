# Simple meson build
project('inih', 'c')

inih_includes = include_directories('.')

inih = static_library(
    'inih',
    sources: [
        'ini.c',
    ],
    include_directories: inih_includes,
    install: false,
)

inih_dependency = declare_dependency(
    include_directories: inih_includes,
    link_with: inih
)
