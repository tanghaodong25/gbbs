cc_binary(
    name = "compressor",
    srcs = ["compressor.C"],
    deps = [
        "//ligra",
        "//ligra:io",
        "//ligra:parse_command_line",
        "//pbbslib:random",
        "//pbbslib:utilities",
    ],
)

cc_binary(
    name = "converter",
    srcs = ["converter.C"],
    deps = [
        ":converter_library",
    ],
)

cc_binary(
    name = "random_reorder",
    srcs = ["random_reorder.C"],
    deps = [
        "//ligra",
        "//ligra:bridge",
        "//pbbslib:random_shuffle",
        "//pbbslib/strings:string_basics",
    ],
)

cc_binary(
    name = "to_edge_list",
    srcs = ["to_edge_list.C"],
    deps = [
        "//ligra",
        "//ligra:bridge",
        "//pbbslib:random_shuffle",
        "//pbbslib/strings:string_basics",
    ],
)

cc_library(
    name = "converter_library",
    hdrs = [
        "converter.h",
        "to_char_arr.h",
    ],
    deps = ["//ligra"],
)
