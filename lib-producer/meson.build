project(
  'lib-producer', 
  ['c', 'vala'],        
  version: '0.1.0',
  meson_version: '>= 0.46.0',
)

pkg = import('pkgconfig')

dependencies = [
    dependency('glib-2.0'),
    dependency('gobject-2.0'),
]

lib_producer = library('lib-producer', 'Library.vala',
        dependencies: dependencies,
        install: true,
        install_dir: [true, true, true])

lib_dependency = declare_dependency(link_with: lib_producer,
                             include_directories: include_directories('.'))

pkg.generate(lib_producer)