package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = ["start.go"],
    tags = ["automanaged"],
    deps = [
        "//cmd/kube-aggregator/pkg/apis/apiregistration/v1alpha1:go_default_library",
        "//cmd/kube-aggregator/pkg/apiserver:go_default_library",
        "//cmd/kube-aggregator/pkg/legacy:go_default_library",
        "//pkg/api:go_default_library",
        "//pkg/client/clientset_generated/clientset:go_default_library",
        "//pkg/client/restclient:go_default_library",
        "//pkg/genericapiserver:go_default_library",
        "//pkg/genericapiserver/filters:go_default_library",
        "//pkg/genericapiserver/options:go_default_library",
        "//pkg/kubectl/cmd/util:go_default_library",
        "//pkg/registry/generic:go_default_library",
        "//pkg/registry/generic/registry:go_default_library",
        "//pkg/runtime/schema:go_default_library",
        "//pkg/storage/storagebackend:go_default_library",
        "//pkg/util/sets:go_default_library",
        "//pkg/util/wait:go_default_library",
        "//vendor:github.com/pborman/uuid",
        "//vendor:github.com/spf13/cobra",
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
