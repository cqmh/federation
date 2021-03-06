load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "client_builder.go",
        "controller_ref_manager.go",
        "controller_utils.go",
        "doc.go",
        "lookup_cache.go",
    ],
    importpath = "k8s.io/kubernetes/pkg/controller",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/golang/glog:go_default_library",
        "//vendor/github.com/golang/groupcache/lru:go_default_library",
        "//vendor/k8s.io/api/apps/v1beta1:go_default_library",
        "//vendor/k8s.io/api/authentication/v1:go_default_library",
        "//vendor/k8s.io/api/core/v1:go_default_library",
        "//vendor/k8s.io/api/extensions/v1beta1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/errors:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/meta:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/fields:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/labels:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/types:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/clock:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/errors:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/runtime:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/sets:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/strategicpatch:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/wait:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/watch:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/authentication/serviceaccount:go_default_library",
        "//vendor/k8s.io/client-go/kubernetes:go_default_library",
        "//vendor/k8s.io/client-go/kubernetes/typed/authentication/v1:go_default_library",
        "//vendor/k8s.io/client-go/kubernetes/typed/core/v1:go_default_library",
        "//vendor/k8s.io/client-go/rest:go_default_library",
        "//vendor/k8s.io/client-go/tools/cache:go_default_library",
        "//vendor/k8s.io/client-go/tools/record:go_default_library",
        "//vendor/k8s.io/client-go/util/integer:go_default_library",
        "//vendor/k8s.io/client-go/util/retry:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/api/legacyscheme:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/api/v1/pod:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/apis/core:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/apis/core/install:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/apis/core/validation:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/serviceaccount:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/util/hash:go_default_library",
        "//vendor/k8s.io/kubernetes/pkg/util/taints:go_default_library",
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
    srcs = [
        ":package-srcs",
        "//vendor/k8s.io/kubernetes/pkg/controller/daemon:all-srcs",
        "//vendor/k8s.io/kubernetes/pkg/controller/deployment/util:all-srcs",
        "//vendor/k8s.io/kubernetes/pkg/controller/history:all-srcs",
        "//vendor/k8s.io/kubernetes/pkg/controller/namespace:all-srcs",
        "//vendor/k8s.io/kubernetes/pkg/controller/nodelifecycle:all-srcs",
        "//vendor/k8s.io/kubernetes/pkg/controller/statefulset:all-srcs",
        "//vendor/k8s.io/kubernetes/pkg/controller/util/node:all-srcs",
        "//vendor/k8s.io/kubernetes/pkg/controller/volume/events:all-srcs",
        "//vendor/k8s.io/kubernetes/pkg/controller/volume/persistentvolume:all-srcs",
    ],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
