cmake_minimum_required(VERSION 3.10.2)

project(DataStructureForPieceWiseLinearCurve)

find_package(ITK REQUIRED)
include(${ITK_USE_FILE})


add_executable(DataStructureForPieceWiseLinearCurve Code.cxx)
target_link_libraries(DataStructureForPieceWiseLinearCurve ${ITK_LIBRARIES})

install(TARGETS DataStructureForPieceWiseLinearCurve
  DESTINATION bin/ITKExamples/Filtering/Path
  COMPONENT Runtime
  )

install(FILES Code.cxx CMakeLists.txt
  DESTINATION share/ITKExamples/Code/Filtering/Path/DataStructureForPieceWiseLinearCurve/
  COMPONENT Code
  )


enable_testing()
add_test(NAME DataStructureForPieceWiseLinearCurveTest
  COMMAND ${CMAKE_RUNTIME_OUTPUT_DIRECTORY}/DataStructureForPieceWiseLinearCurve)

