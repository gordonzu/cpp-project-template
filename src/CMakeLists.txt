add_library(project_lib)

target_sources(project_lib
    PUBLIC
        FILE_SET CXX_MODULES
        FILES
            project.cpp
)

target_compile_features(project_lib PUBLIC cxx_std_20)
