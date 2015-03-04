cmake_minimum_required(VERSION 2.8.3)
project(ranger_description)

find_package(catkin REQUIRED COMPONENTS robot_state_publisher urdf)
# Nothing that can be imported by other modules
catkin_package()


# Instructions to install launch files
install(DIRECTORY launch/
    DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/launch )

# Instructions to install urdf files
install(DIRECTORY urdf/
    DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/urdf)

# Instructions to install config files
install(DIRECTORY config/
    DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/config)
