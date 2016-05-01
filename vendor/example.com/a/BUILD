package(
    default_visibility = ["//visibility:public"],
)
load("@io_bazel_rules_go//go:def.bzl", "go_prefix", "go_library")

go_prefix("example.com/a")

go_library(
    name = "go_default_library",
    srcs = ["main.go"],
    deps = ["//vendor/example.com/a/b:go_default_library"],
)
