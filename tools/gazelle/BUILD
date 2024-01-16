load("@gazelle//:def.bzl", "DEFAULT_LANGUAGES", "gazelle_binary")

gazelle_binary(
    name = "gazelle",
    languages = DEFAULT_LANGUAGES + [
        "@rules_buf//gazelle/buf:buf",
    ],
    visibility = ["//visibility:public"],
)
