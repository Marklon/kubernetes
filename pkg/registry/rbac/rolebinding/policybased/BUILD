package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = ["storage.go"],
    tags = ["automanaged"],
    deps = [
        "//pkg/api/errors:go_default_library",
        "//pkg/api/rest:go_default_library",
        "//pkg/apis/rbac:go_default_library",
        "//pkg/apis/rbac/validation:go_default_library",
        "//pkg/genericapiserver/api/request:go_default_library",
        "//pkg/registry/rbac:go_default_library",
        "//pkg/runtime:go_default_library",
        "//vendor:k8s.io/apiserver/pkg/authorization/authorizer",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
)
