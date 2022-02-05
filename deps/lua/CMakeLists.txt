#这个指令是把整个目录的所有文件作为变量，免得一个一个的加
#aux_source_directory (${PROJECT_SOURCE_DIR}/deps/lua/src LUA_SRC)
#add_library(lua STATIC ${LUA_SRC})


set(LUA_SRC
        src/lauxlib.c
        src/liolib.c
        src/lopcodes.c
        src/lstate.c
        src/lobject.c
        src/print.c
        src/lmathlib.c
        src/loadlib.c
        src/lvm.c
        src/lfunc.c
        src/lstrlib.c
        src/lua.c
        src/linit.c
        src/lstring.c
        src/lundump.c
        src/luac.c
        src/ltable.c
        src/ldump.c
        src/loslib.c
        src/lgc.c
        src/lzio.c
        src/ldblib.c
        src/strbuf.c
        src/lmem.c
        src/lcode.c
        src/ltablib.c
        src/lua_struct.c
        src/lapi.c
        src/lbaselib.c
        src/lua_cmsgpack.c
        src/ldebug.c
        src/lparser.c
        src/lua_cjson.c
        src/fpconv.c
        src/lua_bit.c
        src/llex.c
        src/ltm.c
        src/ldo.c
        )

add_library(lua STATIC ${LUA_SRC})