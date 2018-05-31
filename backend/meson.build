ogon_backend_sources = [
	'dmgbuf.c',
	'protocol.c',
	'transport.c',
	'service.c',
	'keycodes.c',
	'../common/security.c',
]

includes_backend = include_directories('.')

ogon_backend_lib = library('ogon-backend',
	sources: [ogon_backend_sources, generated_backend_proto],
	include_directories: [includes_ogon, includes_generated],
	dependencies: [deps_protobuf_c, deps_protobuf, deps_winpr, deps_freerdp],
	version: ogon_version_full,
	soversion: ogon_version[0],
	install: true
)
