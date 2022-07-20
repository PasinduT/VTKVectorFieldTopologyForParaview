set(classes
  vtkAbstractInterpolatedVelocityField
  vtkAMRInterpolatedVelocityField
  vtkCachingInterpolatedVelocityField
  vtkCellLocatorInterpolatedVelocityField
  vtkCompositeInterpolatedVelocityField
  vtkEvenlySpacedStreamlines2D
  vtkInterpolatedVelocityField
  vtkLagrangianBasicIntegrationModel
  vtkLagrangianMatidaIntegrationModel
  vtkLagrangianParticle
  vtkLagrangianParticleTracker
  vtkModifiedBSPTree
  vtkParallelVectors
  vtkParticlePathFilter
  vtkParticleTracer
  vtkParticleTracerBase
  vtkStreaklineFilter
  vtkStreamSurface
  vtkStreamTracer
  vtkTemporalInterpolatedVelocityField
  vtkVectorFieldTopology
  vtkVortexCore
  )

set(headers
  vtkLagrangianThreadedData.h)

vtk_module_add_module(VectorFieldTopologys
  CLASSES ${classes}
  HEADERS ${headers})

paraview_add_server_manager_xmls(
  XMLS  VectorFieldTopology.xml)