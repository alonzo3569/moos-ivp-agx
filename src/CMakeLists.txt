##############################################################################
# FILE:        moos-ivp-extend/src/CMakeLists.txt
# DATE:        2010/09/07
# DESCRIPTION: CMakeLists.txt file for the moos-ivp-extend source directory
##############################################################################


#============================================================================
# Add the libraries in the current directory to the include path
#============================================================================
FILE(GLOB LOCAL_LIBRARY_DIRS ./lib_*)
INCLUDE_DIRECTORIES(${LOCAL_LIBRARY_DIRS})

#============================================================================
# List the subdirectories to build...
#============================================================================
ADD_SUBDIRECTORY(lib_behaviors-alonzo)
ADD_SUBDIRECTORY(pPoseKeepingX)
ADD_SUBDIRECTORY(uSimMarineX_HWGR)
ADD_SUBDIRECTORY(pThrustControl)
ADD_SUBDIRECTORY(pHelmIvP_IMU)
ADD_SUBDIRECTORY(pNodeReporter_IMU)
ADD_SUBDIRECTORY(pImuHeading)
ADD_SUBDIRECTORY(pPinger)
ADD_SUBDIRECTORY(pMovingPinger)
ADD_SUBDIRECTORY(pSourceLocalization)
ADD_SUBDIRECTORY(pSourceLocalizationFront)

##############################################################################
#                           END of CMakeLists.txt
##############################################################################

