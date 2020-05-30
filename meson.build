project('nanovg', ['c'], 
         version       : '0.1.0',  
         license       : ['ZLIB'],
         meson_version : '>= 0.49.0')

src_nanovg = [
  'src/nanovg.c'
]

inc_nanovg = include_directories('src')

lib_nanovg = static_library('nanovg',
  src_nanovg,
  include_directories: inc_nanovg
)

nanovg_dep = declare_dependency(include_directories : inc_nanovg, link_with: lib_nanovg)