add_subdirectory(libc)
add_subdirectory(goffice)
add_subdirectory(guile-json)
add_subdirectory(gwengui-gtk3)

set_local_dist(borrowed_DIST_local CMakeLists.txt README)
set(borrowed_DIST ${borrowed_DIST_local} ${libc_DIST} ${guile-json_DIST} ${goffice_DIST} ${gwengui_gtk3_DIST} PARENT_SCOPE)
