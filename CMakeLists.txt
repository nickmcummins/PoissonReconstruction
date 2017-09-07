message(STATUS "PoissonReconstruction: Building as a Remote VTK module")

set(Module_SRCS
    Factor.cpp
    MarchingCubes.cpp
    MultiGridOctreeData.cpp
    Geometry.cpp
    MultiGridOctest.cpp
    vtkPoissonReconstruction.cxx
  )

vtk_module_library(PoissonReconstruction ${Module_SRCS})
