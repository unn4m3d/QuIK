project(QuIK)


add_subdirectory(KDL_IK)
add_library(QuIK INTERFACE)
target_include_directories(QuIK INTERFACE ./QuIK/IK ./QuIK/Robot)
target_link_libraries(QuIK PUBLIC orocos-kdl)