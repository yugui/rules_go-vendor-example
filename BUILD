load("@io_bazel_rules_go//go:def.bzl", "go_prefix", "go_binary")

go_prefix("github.com/yugui/example")

go_binary(
    name = "example",
    srcs = ["main.go"],
    deps = [
        "//vendor/example.com/a:go_default_library",
    ]
)
