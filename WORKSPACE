load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

release = "1.24.3"
http_archive(
    name = "com_github_grpc_grpc",
    urls = ["https://github.com/grpc/grpc/archive/v" + release + ".tar.gz"],
    strip_prefix = "grpc-" + release,
)
load("@com_github_grpc_grpc//bazel:grpc_deps.bzl", "grpc_deps")
grpc_deps()
