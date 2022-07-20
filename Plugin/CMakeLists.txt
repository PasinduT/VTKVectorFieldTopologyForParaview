
paraview_add_plugin(VectorFieldTopology
  REQUIRED_ON_CLIENT
  REQUIRED_ON_SERVER
  VERSION "1.0"
  MODULES VectorFieldTopologys
  MODULE_FILES "${CMAKE_CURRENT_SOURCE_DIR}/FlowPath/vtk.module")