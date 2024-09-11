rock_find_qt4(OPTIONAL)
rock_find_qt5(OPTIONAL)

if(ROCK_QT_VERSION_4)
    rock_vizkit_plugin(odometry-viz
        MOC BodyContactStateVisualization.cpp
        DEPS odometry
        HEADERS BodyContactStateVisualization.hpp)
endif()

if(ROCK_QT_VERSION_5)
    rock_vizkit_plugin_qt5(odometry-viz-qt5
        MOC5 BodyContactStateVisualization.cpp
        DEPS odometry
        HEADERS BodyContactStateVisualization.hpp)
endif()

