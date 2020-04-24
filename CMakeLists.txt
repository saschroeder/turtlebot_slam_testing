cmake_minimum_required(VERSION 2.8.3)
project(turtlebot_slam_testing)

find_package(catkin REQUIRED COMPONENTS
  urdf
  xacro
)


catkin_package(
   CATKIN_DEPENDS urdf xacro
)

install(DIRECTORY launch
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
install(DIRECTORY urdf
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
)
