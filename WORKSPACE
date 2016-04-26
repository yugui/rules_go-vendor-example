git_repository(
    name = "io_bazel_rules_go",
    remote = "https://github.com/bazelbuild/rules_go.git",
    commit = "373feb67001252371054c3388291661352c4eb90",
)
load("@io_bazel_rules_go//go:def.bzl", "go_repositories")

go_repositories()

glog_build = """
package(default_visibility = ["//visibility:public"])

load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_prefix")

go_prefix("github.com/golang/glog")
go_library(
    name = "go_default_library",
    srcs = glob(
        ["*.go"],
        exclude=["*_test.go"],
    ),
)
"""

new_git_repository(
    name = "glog",
    remote = "https://github.com/golang/glog.git",
    build_file_content = glog_build,
    commit = "23def4e6c14b4da8ac2ed8007337bc5eb5007998",
)
