# A basic meson.build file needed for using project as a
# meson wrap dependency
project('nanosvg','cpp')

inc = include_directories('src')

nanosvg_dep = declare_dependency(
  include_directories : inc,
)

if meson.version().version_compare('>= 0.54.0')
  meson.override_dependency('nanosvg', nanosvg_dep)
endif
