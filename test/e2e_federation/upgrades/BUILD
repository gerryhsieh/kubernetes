package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "simple.go",
        "upgrade.go",
    ],
    tags = ["automanaged"],
    deps = [
        "//federation/pkg/federatedtypes:go_default_library",
        "//federation/pkg/federatedtypes/crudtester:go_default_library",
        "//test/e2e_federation/framework:go_default_library",
        "//vendor/github.com/onsi/ginkgo:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
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
