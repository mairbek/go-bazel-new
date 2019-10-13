load("@io_bazel_rules_go//go:def.bzl", "go_binary", "go_library")
load("@bazel_gazelle//:def.bzl", "gazelle")

gazelle(
    name = "gazelle",
    prefix = "github.com/mairbek/template",
)

go_library(
    name = "go_default_library",
    srcs = ["main.go"],
    importpath = "github.com/mairbek/template",
    visibility = ["//visibility:private"],
)

go_binary(
    name = "template",
    embed = [":go_default_library"],
    visibility = ["//visibility:public"],
)
