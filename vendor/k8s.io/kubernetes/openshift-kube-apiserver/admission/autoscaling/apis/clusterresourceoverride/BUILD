load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "doc.go",
        "name.go",
        "register.go",
        "types.go",
        "zz_generated.deepcopy.go",
    ],
    importpath = "k8s.io/kubernetes/openshift-kube-apiserver/admission/autoscaling/apis/clusterresourceoverride",
    visibility = ["//visibility:public"],
    deps = [
        "//staging/src/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
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
        "//openshift-kube-apiserver/admission/autoscaling/apis/clusterresourceoverride/v1:all-srcs",
        "//openshift-kube-apiserver/admission/autoscaling/apis/clusterresourceoverride/validation:all-srcs",
    ],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
