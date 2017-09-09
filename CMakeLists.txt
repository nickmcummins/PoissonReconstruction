message(STATUS "PoissonReconstruction: Building as a Remote VTK module")

set(Module_SRCS
    Factor.cpp
    MarchingCubes.cpp
    MultiGridOctreeData.cpp
    Geometry.cpp
    MultiGridOctest.cpp
    vtkPoissonReconstruction.cxx
  )
set_source_files_properties(
    Factor.cpp
    MarchingCubes.cpp
    MultiGridOctreeData.cpp
    Geometry.cpp
    MultiGridOctest.cpp
    PROPERTIES WRAP_EXCLUDE 1
)

vtk_module_library(PoissonReconstruction ${Module_SRCS})
