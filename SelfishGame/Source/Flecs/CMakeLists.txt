
add_library(Flecs
    flecs.c
    flecs.h
    GameWorld.cpp
    GameWorld.h
)

target_include_directories(Flecs PUBLIC
    "${PROJECT_SOURCE_DIR}/Source"
    "${PROJECT_SOURCE_DIR}/Source/Flecs"
    "${PROJECT_SOURCE_DIR}/3rdparty/PhysX5/include"
)

target_include_directories(Flecs
    INTERFACE 
        "${PROJECT_SOURCE_DIR}/Source/Flecs"
)


set_target_properties(Flecs PROPERTIES FOLDER "Selfish")
