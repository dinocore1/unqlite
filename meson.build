project('unqlite', 'c')

if get_option('shared_lib')
  libtype = 'shared_library'
else
  libtype = 'static_library'
endif

src = ['unqlite.c']

incdir = include_directories('.')

unqlite_lib = build_target('unqlite', src,
	include_directories : incdir,
	target_type : libtype,
)

dep = declare_dependency(link_with : unqlite_lib,
	include_directories : incdir
)