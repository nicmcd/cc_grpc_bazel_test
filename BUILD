load("@com_github_grpc_grpc//bazel:cc_grpc_library.bzl",
     "cc_grpc_library",
)

proto_library(
    name = "simple_proto",
    srcs = ["simple.proto"],
)

cc_grpc_library(
    name = "simple_py_pb2_grpc",
    srcs = [],
    deps = [":simple_proto"],
)

cc_binary(
    name = "client",
    srcs = ["client.cc"],
    deps = [
        ":simple_py_pb2_grpc",
    ],
)
