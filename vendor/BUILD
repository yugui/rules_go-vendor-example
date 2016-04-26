package(default_visibility = ["//visibility:public"])

load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "github.com/golang/glog",
    srcs = glob(
        ["github.com/golang/glog/*.go"],
        exclude=["github.com/golang/glog/*_test.go"],
    ),
)


