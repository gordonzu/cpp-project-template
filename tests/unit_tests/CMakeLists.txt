include(GoogleTest)

add_executable(project_tests
    unit_test.cpp
)

target_compile_features(project_tests PRIVATE cxx_std_20)
target_link_libraries(project_tests PRIVATE project_lib gtest gtest_main)

gtest_discover_tests(project_tests)
