project(QuIK)


add_subdirectory(KDL_IK/KDL-1.5.0)
add_library(QuIK INTERFACE)
target_include_directories(QuIK INTERFACE ./QuIK/IK ./QuIK/Robot)
target_link_libraries(QuIK PUBLIC orocos-kdl)
