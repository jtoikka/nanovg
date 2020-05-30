project('nanovg', ['c'], 
         version       : '0.1.0',  
         license       : ['ZLIB'],
         meson_version : '>= 0.49.0')

src_nanovg = [
  'nanovg.c'
]

headers_nanovg = [
  'fontstash.h',
  'nanovg_gl_utils.h',
  'nanovg_gl.h',
  'nanovg.h',
  'stb_image.h',
  'stb_truetype.h'
]

inc_nanovg = include_directories('.')

lib_nanovg = static_library('nanovg',
  src_nanovg,
  include_directories: inc_nanovg
)

nanovg_dep = declare_dependency(include_directories : inc_nanovg, link_with: lib_nanovg)