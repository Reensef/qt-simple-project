enable_testing()

add_compile_definitions(TRANSFORM_TESTEE_CLASS_FOR_UNIT_TESTS)

TEST(TEST_NAME logic_plugin_tests
    DEPENDS
    Qt5Test
    Qt5Quick
    Qt5Qml
    Qt5Core
    Qt5Gui
    Qt5QuickControls2

    OPTIONAL_DEPENDS
    ${PROJECT_NAMESPACE}::core
    ${PROJECT_NAMESPACE}::logic_plugin
    ${PROJECT_NAMESPACE}::gui_plugin
)
