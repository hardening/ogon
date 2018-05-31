generated_ots_thrift = custom_target('gen-thrift-ots',
       input: '../otsapi.thrift',
       output: ['@BASENAME@_types.cpp', '@BASENAME@_types.h',
			 '@BASENAME@_constants.cpp', '@BASENAME@_constants.h',
			 '@BASENAME@.cpp'],
       command: [thrift, '--gen', 'cpp', '-out', '@OUTDIR@', '@INPUT@'],
)

includes_generated_ots = include_directories('..')
