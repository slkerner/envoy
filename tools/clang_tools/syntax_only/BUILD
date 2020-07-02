load("//clang_tools/support:clang_tools.bzl", "clang_tools_cc_binary")

licenses(["notice"])  # Apache 2

# Instructions to build this target are in ../README.md.
# If you do not set the environment variable LLVM_CONFIG as described in that
# file, bazel will fail to build this target.
clang_tools_cc_binary(
    name = "syntax_only",
    srcs = ["main.cc"],
    deps = [
        "@clang_tools//:clang_astmatchers",
        "@clang_tools//:clang_basic",
        "@clang_tools//:clang_tooling",
    ],
)
