cmake_minimum_required(VERSION 3.27)
project(rubiks_cube_solver_main)

set(CMAKE_CXX_STANDARD 14)

include_directories(.)
include_directories(rubiks-cube-solver-main)
include_directories(rubiks-cube-solver-main/Model)
include_directories(rubiks-cube-solver-main/Model/PatternDatabase)
include_directories(rubiks-cube-solver-main/PatternDatabases)
include_directories(rubiks-cube-solver-main/Solver)

add_executable(rubiks_cube_solver_main
        rubiks-cube-solver-main/.idea/.gitignore
        rubiks-cube-solver-main/.idea/modules.xml
        rubiks-cube-solver-main/.idea/rubiks-cube-solver.iml
        rubiks-cube-solver-main/.idea/vcs.xml
        rubiks-cube-solver-main/.idea/workspace.xml
        rubiks-cube-solver-main/Databases/cornerDepth5V1.txt
        rubiks-cube-solver-main/Model/PatternDatabase/PatternDatabase.h
        rubiks-cube-solver-main/Model/RubiksCube.cpp
        rubiks-cube-solver-main/Model/RubiksCube.h
        rubiks-cube-solver-main/Model/RubiksCube1dArray.cpp
        rubiks-cube-solver-main/Model/RubiksCube3dArray.cpp
        rubiks-cube-solver-main/Model/RubiksCubeBitboard.cpp
        rubiks-cube-solver-main/PatternDatabases/CornerDBMaker.cpp
        rubiks-cube-solver-main/PatternDatabases/CornerDBMaker.h
        rubiks-cube-solver-main/PatternDatabases/CornerPatternDatabase.cpp
        rubiks-cube-solver-main/PatternDatabases/CornerPatternDatabase.h
        rubiks-cube-solver-main/PatternDatabases/math.cpp
        rubiks-cube-solver-main/PatternDatabases/math.h
        rubiks-cube-solver-main/PatternDatabases/NibbleArray.cpp
        rubiks-cube-solver-main/PatternDatabases/NibbleArray.h
        rubiks-cube-solver-main/PatternDatabases/PatternDatabase.cpp
        rubiks-cube-solver-main/PatternDatabases/PatternDatabase.h
        rubiks-cube-solver-main/PatternDatabases/PermutationIndexer.h
        rubiks-cube-solver-main/Solver/BFSSolver.h
        rubiks-cube-solver-main/Solver/DFSSolver.h
        rubiks-cube-solver-main/Solver/IDDFSSolver.h
        rubiks-cube-solver-main/.gitignore
        rubiks-cube-solver-main/CMakeLists.txt
        rubiks-cube-solver-main/main.cpp
        rubiks-cube-solver-main/README.md)
