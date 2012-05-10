cmake_minimum_required( VERSION 2.8 )

project( ImageProcessing )

set( CMAKE_BUILD_TYPE "Debug" )

set( CMAKE_CXX_FLAGS_DEBUG "-W -Wextra -g -O0" )
set( CMAKE_CXX_FLAGS_RELEASE "" )

set( CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} 
     /opt/local/share/OpenCV 
     /Users/frferrara/Documents/workspace_cpp/cmake )
     
find_package( OpenCV REQUIRED )
find_package( EIGEN3 REQUIRED )

include_directories( IPInterface
                     StandardIP
                     ImageProcessing )