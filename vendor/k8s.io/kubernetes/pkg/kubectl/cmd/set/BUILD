load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "helper.go",
        "set.go",
        "set_env.go",
        "set_image.go",
        "set_resources.go",
        "set_selector.go",
        "set_serviceaccount.go",
        "set_subject.go",
    ],
    importpath = "k8s.io/kubernetes/pkg/kubectl/cmd/set",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/spf13/cobra:go_default_library",
        "//vendor/k8s.io/api/core/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/errors:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/meta:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/types:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/errors:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/sets:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/strategicpatch:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/validation:go_default_library",
        "//vendor/k8s.io/client-go/kubernetes:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/apis/rbac:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/kubectl:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/kubectl/cmd/templates:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/kubectl/cmd/util:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/kubectl/cmd/util/env:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/kubectl/resource:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/kubectl/util/i18n:go_default_library",
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
    visibility = ["//visibility:public"],
)
