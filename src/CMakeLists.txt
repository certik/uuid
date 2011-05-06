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
