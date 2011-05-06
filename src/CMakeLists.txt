set(SRC
    clear.c
    compare.c
    copy.c
    gen_uuid.c
    isnull.c
    pack.c
    parse.c
    unpack.c
    unparse.c
    uuid_time.c
)

add_library(uuid SHARED ${SRC})

install(TARGETS uuid
    RUNTIME DESTINATION lib
    ARCHIVE DESTINATION lib
    LIBRARY DESTINATION lib
    )
install(FILES uuid.h uuidd.h uuidP.h
    DESTINATION include
    )
