cmake_minimum_required(VERSION 2.8.3)
project(barrett_hand_defs)
find_package(catkin REQUIRED)

catkin_package(CATKIN_DEPENDS xacro)

install(DIRECTORY defs launch meshes robots
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})

#foreach(dir defs launch meshes robots)
#   install(DIRECTORY ${dir}/
#      DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/${dir})
#endforeach(dir)
