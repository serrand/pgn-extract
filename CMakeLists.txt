cmake_minimum_required(VERSION 2.8)
project(pgn-extract)
add_library(pgn-extract apply.c argsfile.c decode.c eco.c end.c grammar.c hashing.c lex.c lines.c lists.c map.c moves.c mymalloc.c output.c fenmatcher taglines.c)
add_executable(main main.c)
target_link_libraries(main pgn-extract)


