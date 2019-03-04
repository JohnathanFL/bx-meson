project('bx', 'cpp')
bxHeaders = include_directories('bx/include')
thirdParty = include_directories('bx/3rdparty')

cpp = meson.get_compiler('cpp')
pthread = cpp.find_library('pthread')
dl = cpp.find_library('dl', required: true)
gl = dependency('GL')


library('bx', 'bx/src/amalgamated.cpp', include_directories: [bxHeaders, thirdParty], dependencies: [dl, gl, pthread])
