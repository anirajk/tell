file(GLOB watchlist RELATIVE ${CMAKE_CURRENT_SOURCE_DIR} *)
foreach(f ${watchlist})
    if(IS_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/${f})
        add_subdirectory(${f})
    endif()
endforeach()
