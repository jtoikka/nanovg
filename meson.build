project('nanovg', ['c'], 
         version       : '0.1.0',  
         license       : ['ZLIB'],
         meson_version : '>= 0.49.0')

src_nanovg = [
  'src/nanovg.c'
]

headers_nanovg = [
  'src/fontstash.h',
  'src/nanovg_gl_utils.h',
  'src/nanovg_gl.h',
  'src/nanovg.h',
  'src/stb_image.h',
  'src/stb_truetype.h'
]

inc_nanovg = include_directories('.')

lib_nanovg = static_library('nanovg',
  src_nanovg,
  include_directories: inc_nanovg
)

nanovg_dep = declare_dependency(include_directories : inc_nanovg, link_with: lib_nanovg)