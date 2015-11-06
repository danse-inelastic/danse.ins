# docker 

configure_file(setup-danse.sh.in setup-danse.sh)
install(PROGRAMS ${CMAKE_CURRENT_BINARY_DIR}/setup-danse.sh DESTINATION bin)