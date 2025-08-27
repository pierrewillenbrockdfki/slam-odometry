rock_find_qt4(OPTIONAL)
rock_find_qt5(OPTIONAL)

include(RockQt)

rock_qt_vizkit_plugin(
    TARGETPREFIX odometry-viz
    QT4_SUFFIX ""
    MISSINGQTDEPS_NOBUILD
    SOURCES BodyContactStateVisualization.cpp
    MOC BodyContactStateVisualization.hpp
    DEPS odometry
    HEADERS BodyContactStateVisualization.hpp)

