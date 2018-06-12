ADD_EXECUTABLE(curltest main.c)

FIND_PACKAGE(curl)

if(CURL_FOUND)
  INCLUDE_DIRECTORIES(${CURL_INCLUDE_DIR})
  TARGET_LINK_LIBRARIES(curltest ${CURL_LIBRARY})
elseif(CURL_FOUND)
  message(fatal_error "CURL library not found")
endif(CURL_FOUND)
