configure_file(app4triqs-config.cmake.in app4triqs-config.cmake @ONLY)
configure_file(app4triqs-config-version.cmake.in app4triqs-config-version.cmake @ONLY)
install(
  FILES
    ${CMAKE_CURRENT_BINARY_DIR}/app4triqs-config.cmake
    ${CMAKE_CURRENT_BINARY_DIR}/app4triqs-config-version.cmake
  DESTINATION lib/cmake/app4triqs
)

install(EXPORT app4triqs-targets DESTINATION lib/cmake/app4triqs)
