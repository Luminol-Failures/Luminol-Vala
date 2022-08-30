luminol_sources = [
  'main.vala',
  'window.vala',
  'application.vala',
]

luminol_deps = [
  dependency('libadwaita-1', version: '>= 1.0'),
]

gnome = import('gnome')

luminol_sources += gnome.compile_resources('luminol-resources',
  'luminol.gresource.xml',
  c_name: 'luminol'
)

executable('luminol', luminol_sources,
  vala_args: '--target-glib=2.50',  dependencies: luminol_deps,
  install: true,
)
