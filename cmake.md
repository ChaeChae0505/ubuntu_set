running command 에 대해 안되는 것인 줄 알았다.
돌고 있다는 말이였다. 
Rospack profile 했을 때 파일 폴더가 안 보이면 그냥 그 창에 source ~/폴더명/devel/setup.bash 하면 된다. 

make -j4 -l4라는 말은 그냥 추천 해주는 것인데 j4가 컴퓨터의 코어 수를 뜻하고 얼마나 사용할 수 있는지 추천 해주는 것

```

####
#### Running command: "cmake /home/a307/ws/src -DCATKIN_DEVEL_PREFIX=/home/a307/ws/devel -DCMAKE_INSTALL_PREFIX=/home/a307/ws/install -G Unix Makefiles" in "/home/a307/ws/build"
####
-- The C compiler identification is GNU 7.5.0
-- The CXX compiler identification is GNU 7.5.0
-- Check for working C compiler: /usr/bin/cc
-- Check for working C compiler: /usr/bin/cc -- works
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Detecting C compile features
-- Detecting C compile features - done
-- Check for working CXX compiler: /usr/bin/c++
-- Check for working CXX compiler: /usr/bin/c++ -- works
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Using CATKIN_DEVEL_PREFIX: /home/a307/ws/devel
-- Using CMAKE_PREFIX_PATH: /home/a307/m_ws/devel;/opt/ros/melodic
-- This workspace overlays: /home/a307/m_ws/devel;/opt/ros/melodic
-- Found PythonInterp: /usr/bin/python2 (found suitable version "2.7.17", minimum required is "2") 
-- Using PYTHON_EXECUTABLE: /usr/bin/python2
-- Using Debian Python package layout
-- Using empy: /usr/bin/empy
-- Using CATKIN_ENABLE_TESTING: ON
-- Call enable_testing()
-- Using CATKIN_TEST_RESULTS_DIR: /home/a307/ws/build/test_results
-- Found gtest sources under '/usr/src/googletest': gtests will be built
-- Found gmock sources under '/usr/src/googletest': gmock will be built
-- Found PythonInterp: /usr/bin/python2 (found version "2.7.17") 
-- Looking for pthread.h
-- Looking for pthread.h - found
-- Looking for pthread_create
-- Looking for pthread_create - not found
-- Looking for pthread_create in pthreads
-- Looking for pthread_create in pthreads - not found
-- Looking for pthread_create in pthread
-- Looking for pthread_create in pthread - found
-- Found Threads: TRUE  
-- Using Python nosetests: /usr/bin/nosetests-2.7
-- catkin 0.7.29
-- BUILD_SHARED_LIBS is on
-- BUILD_SHARED_LIBS is on
-- Configuring done
-- Generating done
-- Build files have been written to: /home/a307/ws/build
####
#### Running command: "make -j4 -l4" in "/home/a307/ws/build"
####
```
