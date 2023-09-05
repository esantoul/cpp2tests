To install dependencies and build the project:
 - install conan (version should be > 2.0.0)
 - conan install . -pr:b conan_profile -pr:h conan_profile --output-folder=build --build=missing -s build_type=Debug
 - cd build
 - cmake .. -G Ninja -DCMAKE_TOOLCHAIN_FILE=conan_toolchain.cmake -DCMAKE_BUILD_TYPE=Debug
 - cmake --build . --config Debug

You can choose the build type among ['Debug', 'Release', 'RelWithDebInfo', 'MinSizeRel']
