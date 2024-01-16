load("@rules_go//go:def.bzl", "go_binary", "go_library")

go_library(
    name = "bes_lib",
    srcs = ["main.go"],
    importpath = "github.com/geethree/bep-to-otel/cmd/bes",
    visibility = ["//visibility:private"],
    deps = [
        "@com_github_golang_protobuf//ptypes:go_default_library_gen",
        "@com_github_golang_protobuf//ptypes/empty",
        "@com_github_pkg_errors//:go_default_library",
        "@org_golang_google_genproto//googleapis/devtools/build/v1:go_default_library",
        "@org_golang_google_grpc//:go_default_library",
    ],
)

go_binary(
    name = "bes",
    embed = [":bes_lib"],
    visibility = ["//visibility:public"],
)
