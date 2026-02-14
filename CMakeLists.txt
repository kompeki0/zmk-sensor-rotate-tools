# CMakeLists.txt (module root)
if ((NOT CONFIG_ZMK_SPLIT) OR CONFIG_ZMK_SPLIT_ROLE_CENTRAL)
  target_sources(
    src/behavior_input_two_axis_oneshot.c
    src/behavior_sensor_rotate_accel.c
  )
  zephyr_include_directories(include)
endif()
