project('vala app', 'vala', 'c')

# vapi_dir = meson.current_source_dir() / 'vapi'

# add_project_arguments(['--vapidir', vapi_dir], language: 'vala')

dependencies = [
    dependency('glib-2.0'),
    dependency('gobject-2.0'),
    dependency('lib-producer'), # 'foo.vapi' will be resolved as './vapi/foo.vapi'
]

sources = files('app.vala')

executable('app-consumer', sources, dependencies: dependencies)