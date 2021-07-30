```
cmake-tutorial % mkdir build
cmake-tutorial % cd build 
# ..は, 1つ下のディレクトリの階層を指す. CMakeLists.txtが存在するディレクトリを指定する
build % cmake ..
CMake Warning (dev) in CMakeLists.txt:
  No project() command is present.  The top-level CMakeLists.txt file must
  contain a literal, direct call to the project() command.  Add a line of
  code such as

    project(ProjectName)

  near the top of the file, but after cmake_minimum_required().

  CMake is pretending there is a "project(Project)" command on the first
  line.
This warning is for project developers.  Use -Wno-dev to suppress it.

-- The C compiler identification is AppleClang 12.0.0.12000032
-- The CXX compiler identification is AppleClang 12.0.0.12000032
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working C compiler: /Library/Developer/CommandLineTools/usr/bin/cc - skipped
-- Detecting C compile features
-- Detecting C compile features - done
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /Library/Developer/CommandLineTools/usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Configuring done
-- Generating done
-- Build files have been written to: /xxxxx/cmake-tutorial/build
# .は, ConfigureとGenerateを実行したディレクトリ, すなわちbuildディレクトリを指す
build % cmake --build .
[ 50%] Building CXX object CMakeFiles/HelloWorld.dir/hello_world.cpp.o
[100%] Linking CXX executable HelloWorld
[100%] Built target HelloWorld
build % ./HelloWorld 
Hello World!
```                                                                                                                                                             
