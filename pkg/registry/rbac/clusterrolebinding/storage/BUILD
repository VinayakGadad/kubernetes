package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = ["storage.go"],
    importpath = "k8s.io/kubernetes/pkg/registry/rbac/clusterrolebinding/storage",
    deps = [
        "//pkg/apis/rbac:go_default_library",
        "//pkg/printers:go_default_library",
        "//pkg/printers/internalversion:go_default_library",
        "//pkg/printers/storage:go_default_library",
        "//pkg/registry/rbac/clusterrolebinding:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//staging/src/k8s.io/apiserver/pkg/registry/generic:go_default_library",
        "//staging/src/k8s.io/apiserver/pkg/registry/generic/registry:go_default_library",
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
