

configure_file(build/Dockerfile build/Dockerfile)
configure_file(build/run build/run)

configure_file(test/Dockerfile.in test/Dockerfile)
configure_file(test/run test/run)

# output under ..../build/SRPMS/
add_custom_target( 
  build-srpm
  COMMAND bash run
  WORKING_DIRECTORY build
  )

add_custom_target( 
  test-srpm
  COMMAND bash run
  WORKING_DIRECTORY test
  )
